# This is a cool webring thing.

[Test Page](https://tekgo.github.io/simpleWebRing/test.html)

## Joining the web ring:
Have a cool website. Submit a pull request to this repo adding yourself to the `sites` list.

You'll need the following info:
- A unique id to use for your link.
- A title for your link.
- A url for your link.

## Embedding instructions:

### iFrame
This will include the links inside an embeddable frame you can just put on your page. Just include the followiing code replacing `<your-id-here>` with your link's id:

```
<iframe src="https://tekgo.github.io/simpleWebRing/#id=<your-id-here>" width="500" sandbox="allow-scripts allow-top-navigation"></iframe>
```

### Text links
You can also include the links as raw html inside your page so you have more flexibility in their display. Here is an example of them as a list:

```
<ul>
	<li><a href="https://tekgo.github.io/simpleWebRing/#id=<your-id-here>&redirectMode=prev">previous</a></li>
	<li><a href="https://tekgo.github.io/simpleWebRing/#id=<your-id-here>&redirectMode=next">next</a></li>
	<li><a href="https://tekgo.github.io/simpleWebRing/#id=<your-id-here>&redirectMode=random">random</a></li>
</ul>
```

## Customization:
