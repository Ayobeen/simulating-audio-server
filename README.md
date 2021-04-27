# python-flask-coding-exercise
A Flask Web API that simulates the behavior of an audio file server
## Features
consummers can send
- get request
- send post request
- send update request
- delete audio request

<h3>API CONSUMPTION</h3>

<P><b>WEB URL </b>
    https://filedaudioserver.herokuapp.com/</P>

    <h3>API ENDPOINTS FORMAT</h3>
<p>filedaudioserver.herokuapp.com/api/v1/resources/audiotype
	<br>
    for all audio<br>
filedaudioserver.herokuapp.com/api/v1/resources/audiotype/id
	<br>
    for single audio<br>
	where id = 1,2,3,.....</p>

<h3>GET REQUEST</h3>
<p>filedaudioserver.herokuapp.com/api/v1/resources/song<br>
	return all song<br>
filedaudioserver.herokuapp.com/api/v1/resources/podcast<br>
	return all podcast<br>
filedaudioserver.herokuapp.com/api/v1/resources/audiobook<br>
	return all audiobook<br>

filedaudioserver.herokuapp.com/api/v1/resources/song/id<br>
	return single song<br>
	where id = 1,2,3,.....<br>
	same for podcast and audiobook just change the song in the url to podcast and audiobook respectively
</p>

<h3>FOR POST REQUEST</h3>
<p>
url = filedaudioserver.herokuapp.com/api/v1/resources/audiotype<br>
where audiotype at the end of the url be replaced with "song" or "podcast" or "audiobook"<br>
and the body of the request for each adiotype are:<br>

<b>for song audiotype, use this format</b><br>
	{<br>
        "name_of_song": "I'm the name",<br>
        "duration": 36,      <br>
    }<br>

<b> for podcast audiotype use this format</b><br>
	{<br>
        "name_of_podcast": "I'm the name",<br>
	"duration": 36,<br>
        "host": "Brian",<br>
        "participants": "Brian, Mumeen Updated"<br>
    }<br>

<b>for audiobook audiotype us this format</b><br>
	{
        "title_of_audiobook": "I'm the title",<br>
        "duration": 36,<br>
        "narrator": "Abdlazeez",<br>
        "author": "Brian, Mumeen"<br>
           
    }<br>
</p>

<h3>FOR UPDATE AND DELETE REQUEST</h3>
<p>
use the same request body format as post request except adding the id of the audio to be deleted to the end of the url
<br>
url url = filedaudioserver.herokuapp.com/api/v1/resources/audiotype/id
</p>
Live link https://filedaudioserver.herokuapp.com
