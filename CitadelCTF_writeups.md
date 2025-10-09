# Shinsu DexQuest
As you climb the path, a guardian emerges, its form shifting between the visage of a long-dead climber and a metallic sentinel. It moves with a strange grace, holding out a cartridge containing a single file. You realize the file is compatible with the device you carry and may be the key to continue your ascent toward the Citadel’s heart.

Attachments: `dexquest.apk`

## Exploring the App

Upon running the `.apk` on an Android device (or emulator), the landing page displays a cryptic description and a central doorway.
Swiping across the screen reveals multiple “rooms”:

### Swiping Left - Shinsu Barrier
- Contains a button labeled “Enter Barrier”.
- Pressing it crashes the app with the Toast message:
  “You were absolutely deep fried by the barrier.”
- If you swipe further left, you briefly see a Minecraft-like room containing a flag made of blocks with a prompt `<FLAG>` — the final destination.

### Swiping Right - Sealed Observer
- Shows a Minecraft observer block and a button labeled “OBSERVE THE OBSERVER”
- Clicking it opens a text input box that reacts differently depending on your entry, for example:
  `Correct: n Probably ¯\_(ツ)_/¯` where `n` is a number.
- These clues suggest that the correct numeric input must be derived using JADX.

## Solution

By analyzing the source code at sources/com/shinsu/dexquest/screens/Vault.java in JADX, we can uncover the solution for the Sealed Observer.

- The goal is to make the 'green' variable equal 99, which grants the user the Shinsu Stabilizer Crystal and unlocks the next level. The value of green is determined by the output of the `correctDigits` function, which processes the player's input.
- This function validates the input by checking it digit-by-digit against a specific, hardcoded number. We can replicate this checking logic in a different programming language to find the correct number.
- Once found, you enter this number on the Sealed Observer page to get the Shinsu Stabilizer Crystal. You then take the crystal to the Shinzu Barrier and enter. This action redirects you to a screen with a Minecraft flag, which is copied to your clipboard when you click on it.

**Flag**: `citadel{f33ls_g00d_to_n0t_g3t_d33p_fr13d}`


# Field Day
Deep within the fortified citadel, ancient UNIVAC mainframes hum with classified transmissions. You have spent days infiltrating the Citadel's military grade communication defenses and manage to intercept a FIELDATA transmission encoded onto one of the first methods of storing data. However the data is trapped behind a peculiar digital representation of the FIELDATA encoding, different from the usual 6 bit pairing. Decode the 12 bit transmission to uncover the resistance's secret message.

Attachments: `transmission.txt` Flag Format: `citadel{decodedtransmission}`

## Solution
- The question mentions the FIELDATA format, and looking for `UNIVAC FIELDATA`
- The data should be interpreted as if it were on an 80-column punched card, which has 12 rows for each column.
- Every column represents a character encoded by a 12-bit value. A 1 signifies a punched row, while a 0 signifies an unpunched row. The rows follow a specific order: 12, 11, and then 0 through 9.
- This system uses the military FIELDATA protocol, which features a unique method for handling text case. The [ character combination signals a switch to lowercase for all subsequent characters, while the ] combination reverts the text back to uppercase.

Since we were not very well versed with coding, we decoded the the binary manually. Upon rigourous computation we got the flag.

### Flag: `citadel{r3b3ll10n$&BU1lt:0nH0p3}`


# Viral Bionic Anomaly 
This floor is haunted by a phantom of the past. You encounter a presentation created by the last employee of a forgotten corporation, made just minutes before the Citadel awoke.

Rumor has it that the corporation predicted the rise of the Citadel. Within the slides, a "starter pack" holds the clues you need. Use it to confront the "final boss," a threat trapped inside a macro hidden deep within the presentation, and claim the key to the next floor.

##   Solution
When we open the ppt we find a macro is linked to it. Opening the ppt in ms powerpoint and navigating to the `view` tab followed by the `macro` option, we see a `RunPayload` named macro. Double click it to see the VBA script for it.

In the VBA script we can see 3 main functions - `ZqL9D8`, `JvQ1g` and `Yu89`. They are called in `RunPayload` and their output is concatenated to form flag.

The flag's encryption logic is split across three functions. To decrypt it, we must reverse their processes:

* **Function `ZqL9D8`**: Concatenates 21 encrypted strings and decodes the result from `Base32`.
* **Function `JvQ1g`**: Concatenates 26 encrypted strings and decodes the result from `Base16`.
* **Function `Yu89`**: Concatenates 18 encrypted strings and decodes the result from `Base64`.

Once this overall logic is reversed to get the flag data, we find that its first few bytes are `FF D8 FF E0`. These are the "magic bytes" that identify a file as a `JPG` (as they represent `JFIF` in ASCII).

Therefore, the decrypted data must be saved as a `.jpg` file to reveal the contents.

### Recovering the flag

#### Decoding each function

- Copy-paste all a1 to a21 into one string
- Use cyberchef to convert from Base32
  (CyberChef -> From Base32)
- Save the output as part1.bin

- Copy-paste all b1 to b26 into one long hex string
- (CyberChef -> From Hex)
- Save the output as part2.bin

- Concatenate C1..c18 into one base64 string
- (CyberChef → From Base64)
- Save the output as part3.bin

 
 #### Concatenate the 3 decoded parts and analyze
 
 > ` cat part1.bin part2.bin part3.bin > flag_full.bin`
see the hex code the `flag_full.bin` using
 > `xxd flag_full.bin`

the first bytes are:
`FF D8 FF E0`
That equals JFIF / JPEG magic bytes.

so we now need to rename out file with a .jpg extension
> `mv flag_full.bin flag.jpg`

opening the image we can read the flag 

### Flag: `citadel{gr4b_y0ur_l4bubus_m4tch4s_4nd_dub41_ch0c0l4t3s_y0u_4r3_1n_f0r_4_r1d3}`
 


