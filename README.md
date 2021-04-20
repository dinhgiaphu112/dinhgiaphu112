- 👋 Hi, I’m @dinhgiaphu112
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
dinhgiaphu112/dinhgiaphu112 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

[scheme]://[command]?[params]&[app]&[id]&[callback]
Where:
[scheme] is the wallet's deeplink scheme. Default is trust.
[command] is the command to be executed.
[params] is the command parameters encoded as url query items.
[id] is the unique command id. The value is later used to resolve the callback for the command. Can be any incrementing integer.
[app] callback URL scheme.
[callback]callback path. Default is sdk_sign_result.
Trust will open following URL format if command is succeeded:
[app]://[callback]?[id]&[params]
Where:
[params] is the response parameters, see Parameters section below for each command
Error response format:
[app]://[callback]?[id]&error=[error type]&message=[error message]
pleaes refer to Error Handling for more details.
