# RCompilerBot
Run your R calculations without leaving Telegram 😃

🔗 Link - https://t.me/rcompilerbot

### What can this bot do?
☑️Usage: Start bot and send him any R script. Example: print("hi") <br>
🐞No image/plot support. Calculations only! <br>
🛠Bot is on Alpha stage <br>
👨‍💻Contact admin: @Said_Alphv <br>

![image](https://github.com/fromgodd/RCompilerBot/assets/97128346/30812f99-087f-4474-b370-ae2ef2853eaf)



### How bot works
Generally, infrastructure is not complex. When you send code to bot, it does preprocess to raw text and sends output to temp .R file that is created inside /tmp/. For each user unique temporary folder generated with built-in encryption. Example is User A executes script -> new temp.R created in /tmp/abcde123, but for User B temp.R will be created in /tmp/defgh345 as an example. Execution is working based on subprocess module and spawning R language interpreter from system and specifying temp.R as argument. Everything works under Docker container in safe environment, bot has built-in loop protection but I am working on fixing detailed safety issues and would appreciate any kind of pull requests with bugs and etc.
