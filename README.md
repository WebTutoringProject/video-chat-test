# Custom React video app with Daily React

This is the initial idea for how the call can work using Daily:
https://docs.daily.co/reference/daily-react

# Install
You will need to clone the repo and make sure you have installed `Node.js` and `npm`.
Whether you have Windows or Mac (I am using a Windows 10 VM), you just need to get the Node.js installer.
Once that is installed, write in the terminal of the project `npm install`.

If all goes well and there is no security faults, start npm by writing `npm start`.

When the browser automatically opens (if not, open to `http://localhost:3000`) and ypu get an error when starting a call, it means the api in the `.env` file is invalid. You will need to create a Daily API key by making an account on their website:
https://dashboard.daily.co/developers

Once you get your new API key, replace the `REACT_APP_DAILY_API_KEY` in the `.env` file with your own key.

For the future, we will probably be using Netlify for the React app deployment.

# Notes

Got this while looking to create a local call.

Test call code:
<script crossorigin src="https://unpkg.com/@daily-co/daily-js"></script>
<script>
  callFrame = window.DailyIframe.createFrame();
  callFrame.join({ url: 'https://pricktest.daily.co/hello-daily' });
</script>
