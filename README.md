# Automation of work using GitHub Actions
This is a simple example shows how to automate taking data via API and sending it to a Telegram channel.

 - We get weather data from **API** https://api.open-meteo.com/v1/forecast
 - Convert data into a **Pandas** dataframe 
 - Send data to **Telegram** channel with bot
 - Set up a launch schedule for our application in **GitHub Actions**

## Installation
1. Clone code
2. Create python venv
3. Install Dependencies run ``` pip install -r requirements.txt ```
4. Create .env with your keys
5. Run localy 

### Setting up a schedule

In the file `/.github/workflows/run_daily.yml` after the parameter `on` specify one of the parameters: 
 
 - `push` - one-time launch on push to github repo
 - `workflow_dispatch` - manual start
 - `0 * * * *` - scheduled launch 1 time per hour


## License

**MIT** ©