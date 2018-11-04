# bashbot
<h3>Description: BashBot is a Messaging Client for Slack</h3>

<h1>How to use the bashbot tool</h1>
Usage: bashbot [options] [channel] [message]
  <br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;Options:    **No Options Required**
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-h    Help
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-l    List All Channels in slackchannel.properties
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-a    Add a new channel to slackchannel.properties.  You will need to pass the channel name and url.
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e.g. bashbot -a [new-channel-name] [url]
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-u    Updates an existing channel to slackchannel.properties.  You will need to pass the channel name and url.  If an existing channel can not be found it will add the channel.
  <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;e.g. bashbot -a [existing-channel-name] [url]
  <br>
  &nbsp;&nbsp;&nbsp;&nbsp;e.g. bashbot general "BashBot is Watching... Always Watching"

<b><h1>How to setup slack and the bashbot</h1></b>
1. Establish the 'bashbot' app (substitute your own name if you desire) or use an existing application. Visit <a href="https://api.slack.com/apps">Slack Apps</a> to see existing registrations / create a new app.
2. Once your app is setup, go into your app from <a href="https://api.slack.com/apps">Slack Apps</a> page.
3. Setup 'Incoming Webhooks' for each channel you with to post to.  Each channel will need to be registered and after registration a unique url will be issued for posting to the slack channel.
4. After setting up the 'Incoming Webhooks', use the channel names and matching URL's to add to the slackchannel.properties.  Use the -a or -u option to add the definitions.
