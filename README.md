Splash-Screen
==
#### A Polymer splash-screen element to ease loading UX on any device.

## Demo

Refresh the page to try it out: [Demo](http://duttaoindril.github.io/splash-screen).

## Documentation

### Download the splash-screen.html file and import it in your `index.html`:

`<link rel="import" href="bower_components/duttaoindril/splash-screen.html">`

### Then put this as a child node to your `<body>` tag:

`<splash-screen img-src="<RELATIVE IMAGE PATH>" back-color="<CSS COLOR>"></splash-screen>`

##### NOTE: If your `<body>` tag has an `unresolved` attribute, like so: `<body unresolved>`, please remove it -  otherwise the splashscreen may not show up properly.

### There are also more properties that can be added to the `<splash-screen>` tag:

#### The following convention is followed:

`Name=defaultValue` - Description

#### Properties:

`rippleDisplay="initial"` - Can be set to "none" for no ripples at any time; ripples are always cancelled on a desktop browser.

`anim-delay=1000` - Milliseconds of time the loader will stay on the screen after all content is loaded, useful to hide API requests.

`fade-time=1000` - Milliseconds of time it takes for the entire splash-screen to fade away.

`ripple-freq=250` - Milliseconds of delay between each simulated ripple.

`icon-size=200` - Pixels of the diameter of circle logo, recommended to be at 200px for all screen sizes.

`spinner-sub=5` - Pixels of distance inward the spinner will be from the logo,  can be made negative to have spinner outside the logo.

## Setting up Dependencies

###EITHER:
[Download](https://github.com/PolymerElements/polymer-starter-kit/releases/download/v1.3.0/polymer-starter-kit-1.3.0.zip) the [Polymer Starter Kit](https://github.com/PolymerElements/polymer-starter-kit) and follow it's intstructions to set up a starter Polymer Website, and follow the instructions above to try the element out in the polymer starter kit.

###OR:
Create a Polymer website that has the following dependencies in the `bower_components` folder of dependencies. Acquire these from the [Google Element Catalog](https://elements.polymer-project.org/).

`"bower_components/polymer/polymer.html"`

`"bower_components/paper-spinner/paper-spinner.html"`

`"bower_components/paper-ripple/paper-ripple.html"`

`"bower_components/neon-animation/neon-animation-runner-behavior.html"`

`"bower_components/neon-animation/animations/fade-out-animation.html"`

#### Then...

1.  Download and install Node from [https://nodejs.org/](https://nodejs.org/). Node includes the node package manager command, `npm`.

2.  Install `bower` and `polyserve`:

        npm install -g bower polyserve

3.  Change directory to your local repo and install dependencies with `bower`:

        cd polymer-first-elements
        bower install

4.  To preview the splash-screen element, run `polyserve` from the repo directory:

        polyserve

Open `localhost:8080` in your browser.

If you're wondering what `polyserve` does, see [Testing elements with local bower dependencies](https://www.polymer-project.org/1.0/docs/start/reusableelements.html#local-dependencies)
in the Polymer docs.
