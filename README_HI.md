# NEXORA AI — Android starter prototype

## Is version mein kya kaam karta hai?
- Premium dark/silver Compose interface
- Hindi speech recognition launch (Android speech service par nirbhar)
- Hindi text-to-speech reply (device TTS engine par nirbhar)
- YouTube, WhatsApp, Gmail aur Chrome kholne ke demo commands
- Local note memory: `note kal client ko call karna`
- Saved note dekhna: `note dikhao`
- Time aur help commands

## Abhi kya nahi hai?
- Ye full JARVIS ya general-purpose online AI nahi hai. Brain local rule-based demo hai.
- Wake phrase/background always-listening abhi nahi hai.
- Accessibility service, screen automation, notification reading, calls/SMS sending aur cloud AI backend abhi add nahi kiye gaye.
- Voice recognition may send audio to the speech service configured on the device. Review Android/Google speech settings and privacy choices.

## Sirf Android phone se build karne ke steps
1. Reliable source se AndroidIDE install karein aur app ko open karein.
2. Is ZIP ko phone ke Downloads folder mein extract karein.
3. AndroidIDE mein `NEXORA_AI_Starter` project folder open/import karein.
4. Project sync hone dein. Gradle/JDK/SDK installation maange to AndroidIDE ke supported setup prompts follow karein. Internet pehli build ke liye chahiye ho sakta hai.
5. Build/Run se debug APK banayein.
6. Android prompt aaye to sirf trusted project ka APK install karne ke liye required install permission dein.
7. App khol kar microphone permission allow karein; `YouTube kholo`, `WhatsApp kholo`, `note client ko follow-up karna`, `note dikhao` try karein.

## Agar build fail ho
- AndroidIDE ka exact error text/screenshot share karein.
- AndroidIDE versions ke hisaab se Gradle, JDK aur SDK compatibility badal sakti hai; project sync error ke mutabiq version adjust karna pad sakta hai.

## Security
- App arbitrary shell commands execute nahi karta.
- Sensitive actions ke liye explicit confirmation design karein.
- AI API key kabhi APK/source code mein hard-code na karein. Online AI ke liye backend proxy use karein.
- Accessibility service powerful permission hai: sirf transparent, user-enabled features ke liye use karein.
