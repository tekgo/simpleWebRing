# This is a cool webring thing.

[Test Page](https://tekgo.github.io/simpleWebRing/test.html)

## How it works:
This webring works via a single HTML + Javascript page that can be hosted anywhere. The single page handles the following modes:
- Hub mode, a normal webpage that displays info about the web ring and lists the member sites.
- Embed mode, when embedded as part of an iframe it has the links to the previous/next/random member pages in the ring.
- Redirect mode, all redirects from one ring member to another are handled by this page. This allows member sites to have more customizable ways of displaying the links. This also means that individual member sites don't have to update anything when new members are added.

Because the ring works off a single HTML page it can be hosted almost anywhere and does not require any code to be executed server side. Visitors to the ring are required to have Javascript enabled.

## Forking this project:
You can easily fork this project to make your own web ring. You'll need to make the following changes:
- Update any references to this repo to your own. Especially the base url where your ring will be hosted.
- Customize the `index.html` style for your own ring.
- Edit the `sites` list in `index.html` for your list of member sites.

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
