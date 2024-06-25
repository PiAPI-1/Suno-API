# Suno-API
Introducing our unofficial [Suno API](https://piapi.ai/suno-api), tailored for developers to bring Suno's text-to-music generation to their AI platforms. This integration allows users across the globe to express their musical creativity with ease.
<br><br>

<img src="https://github.com/PiAPI-1/Suno-API/assets/173328932/74a24cf6-c0d2-4ded-a735-e79221c60a05" alt="screenshot of the Midjourney API page from PiAPI" width="95%"/>

<br><br>

<h2>Features</h2>
<ol>
  <li>Integration Ready for V3</li>
  <li>Unlimited Music Creation!</li>
  <li>Asynchronous API Calls</li>
  <li>Suno Lyrics Generation</li>
  <li>Extended clip feature supported!</li>
  <li>Full Access to Advanced API Features</li>
  <li>High Concurrency</li>
  <li>Full song feature supported!</li>
  <li>Pay-as-you-go and Host-your-account Options</li>
  <li>Bulk generation available</li>
</ol>

<br><br>

<h2>Usage Options</h2>

<h3>Pay-as-you-go Option</h3>

<p>
  To get started, simply sign up and purchase credits in our Workspace. Once done, you can immediately access our API! Our service leverages PiAPI’s Suno account pools, ensuring seamless operation without any hassle on your part.
</p>

<ul>
  <li>No need for your own Suno account(s) pool</li>
  <li>No need to manage or operate Suno accounts</li>
  <li>Full access to all endpoints</li>
  <li>Start integrating the API immediately!</li>
</ul>

<br>

<h3>Host-your-account Option</h3>

<p>
  When you choose our Host-Your-Account service, you'll use your own Suno Account(s). Then you can subscribe to PiAPI's Suno API seat(s), connecting your Suno account(s) to the seat(s), and you're ready for integration!
</p>

<ul>
  <li>Faster generation time</li>
  <li>Supports hosting of multiple accounts</li>
  <li>Stable API service</li>
</ul>

<br>

<h3>Pricing</h3>

<h4>Pay-as-you-go Option</h4>

<ul>
  <li>Generation API Call: <b>$0.02</b>/call</li>
  <li>Continuation API Call: <b>$0.02</b>/call</li>
  <li>Lyrics Generation: <b>Free</b></li>
</ul>

<h4>Host-your-account Option</h4>

<ul>
  <li>$<b>5</b>/seat/month</li>
</ul>

<br>

Please refer to our <a href="https://piapi.ai/pricing">pricing page</a> for more information. 

<br><br>

<h2>Usage Steps</h2>

<h3>Pay-as-you-go Option</h3>

<ul>
  <li>Register for PiAPI's Workspace using your GitHub account.</li>
  <li>Obtain your API KEY from our <a href="https://app.piapi.ai/">Workspace</a></li>
  <li>Start coding right away!</li>
</ul>

<br>

<h4>Sample API Calls (using cURL)</h4>

<br>

<p>Create a "Generate Music" call</p>

```
curl --request POST \
  --url https://api.piapi.ai/api/suno/v1/music \
  --header 'Accept: application/json' \
  --header 'Content-Type: application/json' \
  --header 'X-API-Key: {{x-api-key}}' \
  --data '{
  "custom_mode": true,
  "mv": "chirp-v3-5",
  "input": {
    "prompt": "Add_lyrics_into_the_music.",
    "title": "Add_the_title_of_the_song.",
    "tags": "Add_the_type_of_music.",
    "continue_at": 0,
    "continue_clip_id": ""
  }
}'
```
<p>Response</p>

```
{
    "code": 200,
    "data": {
        "task_id": "record_this_taskID"
    },
    "message": "success"
}
```
<br>

<p>Get the "Generate Music" call</p>

```
curl --request GET \
  --url https://api.piapi.ai/api/suno/v1/music/Insert_the_taskID_here \
  --header 'Accept: application/json' \
  --header 'X-API-Key: {{x-api-key}}'
```
<br>

<p>Response - Check out our <a href="https://piapi.ai/docs/faceswap-api/fetch">documentation</a> for more information!</p>

<br><br>

<h2>Contact us</h2>

<p>Email: <a href="mailto:contact@piapi.ai">contact@piapi.ai</a></p>

<br>
