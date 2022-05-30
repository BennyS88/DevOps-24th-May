Create a GitHub repository that executes a workflow each time someone commits a change.

<ul>
  <li>some action is triggered once someone commits a change in the repository</li>
  <li>the GitHub repo link (and README.md file) gives sufficient explanation of what you're trying to achieve, your learning, the steps you take etc.</li>
</ul>

Objective : Sending A Telegram Message When A Push or Pull Request occurred.

<br> Step 1 : Create New Repository
<br> Step 2 : Create README.md
<br> Step 3 : Create .github/workflows/NAME.yml (replace name as you see fit)
<br>
<br> Step 4 : Copy the workflow code from my workflow code
<br> Step 5 : Setup your telegram bot account from https://t.me/botfather
<br> Step 6 : in GitHub, go to settings > Secrets > Actions
<br>  - Add "TELEGRAM_TOKEN" (from Telegram BotFather) and "TELEGRAM_TO" (your bot ID)
<br>
<br>Once the above steps are done, any Push or Pull Requests will be notified to you by the telegram bot.
<br>
<br>The trickiest part : How to get your bot ID
<br> Step 1 : open your terminal
<br> Step 2 : run the following curl request, replace "TOKEN" with your Telegram BotFather Token =
<br>  curl https://api.telegram.org/botTOKEN/getUpdates
<br> Step 3 : your bot ID will be shown from there.
