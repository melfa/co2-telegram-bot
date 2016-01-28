CO2 detector (Masterkit MT8057) telegram bot

# Setup php service

* `apt-get install php5-cli`
* `cd app && nohup php app.php > app.log`

# Setup ngrok https forwarding (for telegram bot API webhook)

* `apt-get install unzip`
* download ngrok from https://ngrok.com/download && unzip
* setup token: `./ngrok authtoken <your_token>`
* run ngrok: `./ngrok http 18062`
* setup telegram https webhook using ngrok: `curl -v https://<your_subdomain>.ngrok.io/setup`
