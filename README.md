# OpenVisConf2016-Notes

Soso sent me to Boston for [OpenVis Conf](https://openvisconf.com/), in April 2016.
Here are my notes.

## Community notes of the talks

https://docs.google.com/document/d/104HDHnXz5G9VIKeG-03OVfTTtvi0c9q0DCMDCtHg3-k/

## My notes

### Talks

> _Legend_:
:eyes: = to look into more
:fire: = awesome!
:bulb: = future experiment idea

#### Seeing Machines Think
> Fernanda Viégas ([@viegasf](https://twitter.com/@viegasf)) and Martin Wattenberg ([@wattenberg](https://twitter.com/wattenberg))

- Their topic today: Neural Nets
  - made of: "filters" and "activations"
  - modeled after the brain and neural networks (duh)
  - secrect: no one really understands neural networks...
- Ingredients of Machine Learning (ML)
  - architecture of the system
  - data
    - _your data is extremely important!_
    - start by looking at your data (_do some datavis!_) before inputting it into ML, to make sure you have:
      - good distribution
      - correct/all types of examples of each "feature"
      - no errors of classifications
      - etc...
- How ML can be fooled
  - "Rubbish examples"
    - Gerhard Richter painting classifies as a “Frog” with 67% confidence
  - "Adverserial examples"
    - changing 1 pixel in a horse image makes the ML think it is now a truck!

:eyes: : http://playground.tensorflow.org/ (was an internal tool @ Google)

__MY OPINION:__ :smile:
  - very good intro to ML for a beginner like myself, chains well with Kyle's talk afterwards (good conf planning)
  - no complaints about the talk; clear, concise, speakers are knowledgeable, not boring

---

#### A Return to Machine Learning
> Kyle McDonald ([@kcimc](https://twitter.com/kcimc))

- Talked about
  1. Convolutional Neural Networks
    - ML hype started with [Deep Dream images](https://vice-images.vice.com/images/articles/meta/2015/07/29/no-they-dream-of-puppy-slugs-0000703-v22n8-1438186190.jpg?resize=*:*&output-quality=75) popping up on the webs
    - demoed his [smile detection project](https://github.com/kylemcdonald/smilecnn) that uses his [ofxCCV](https://github.com/kylemcdonald/ofxCcv) library that names things it sees on webcam using ML (uses another lib called 'CCV' in the background)
      - using Jupyter website for demo, Keras intead of TensorFlow, also uses Theano (?)
  2. Recurrent Neural Networks
    - using [kaparthy's github repo](https://github.com/karpathy) for RNN
    - can create new Shakespeare piece after traning it on all of Shakespeare's work
    - also using it to recreate SVG code using RNN and see what it makes! __AWESOME__ :fire: :bulb:
      - :eyes: : [@GlitchLogos](https://twitter.com/glitchlogos)
      - :eyes: : [Smiling face withface](http://smiling-face-withface.tumblr.com/)
  3. Dimensionality Abstraction/Obstruction
    - uses word2vec

__MY OPINION:__ :blush:
  - not as crazy and fast as I expected, pretty well-spoken, not really structured, but fun
  - I feel like this was fun at the time, but not very memorable; maybe because his stream-of-consciousness style isn't necessarily super education/didactic
  - inspiring and showed me new things, but didn't "learn" too much

---

#### Drawing on \<canvas> - how computers read pixels
> Mariko Kosaka ([@kosamari](https://twitter.com/kosamari))

Quote:
> "knitting *__is__* coding" :fire:
(when talking about pushing & popping threads onto a crochet needle)

- [slides](http://kosamari.com/presentation/openvis-2016)
- whole talk = using \<canvas> to turn manipulate images (and their pixels), write image filters, export pixel data to do other stuff with (like mechanical knitting (not explained))
- she's written many small JS libraries to manipulate images

__MY OPINION:__ :blush:
  - nice talk, knowledgeable about writing basic filters in the web and going between web/machines, interesting
  - I know she has given many other talks, perhaps some more focused on how to achieve the knitting thing, but this one seemed like a bit of a hodge-podge/collection of various little manipulations. That's not bad, but a little fragmented. Cool enough.

---

#### How To Simulate The Universe, In 134 Easy Steps
> Nicky Case ([@ncasenmare](https://twitter.com/@ncasenmare))

- [slides](http://ncase.me/OVC2016/)
- She/he is into 'systems theory'
  - "According to systems thinking, 'The world’s not linear, it’s loopy.'"
  - discovering the truth behind the data
  - removing the noise from the signal
  - social causes, sexism, political strife, violence, racism => systems theory
  - == trying to understand why the data is the way it is
- :eyes: her own example project : [Parable of the polygons](http://ncase.me/polygons/)
  - "empathy" is becoming a watered-down buzzword...
  - __empathy__ is too individual, when used as a solution to human issues
  - __the system__ is our common ennemy
  - project is about how small individual biases in your local neighborhood can affect the larger system
- 5 tools for making systems with stories
  - Old narrativity tools:
    - The Wire, especially 1st season: showing same story from different points of view
    - [Chris Ware, Building Stories (book)](http://www.amazon.com/Building-Stories-Pantheon-Graphic-Novels/dp/0375424334)
    - Vonnegut, Breakfast of Champions (book)
  - Causal Loop Diagrams:
    - [explaning the war on heroin](http://linchpin.org/site/wp-content/uploads/2012/12/Heroin-3.jpeg)
  - Stock and Flow Models:
    - [machine that illustrates the functioning of the economy](http://nzier.org.nz/about/monia-machine/)
  - Probability Simulations: see community notes
  - Agent-Based Modeling: see community notes

__MY OPINION:__ :blush:
  - good social motives to his use of datavis, interesting theoritical backbone to his material (on systems theory) which was high-level but also seemed quite knowledgeable about
  - didn't learn any techniques, per se, but some good examples and leads for building experiences with narrativity and visual explanations of complex systems

---

#### Do you know Nothing when you see it?
> Amelia McNamara ([@AmeliaMN](https://twitter.com/AmeliaMN))

- is a statistics professor
- mentions a free book about randomization techniques
  - talk = using randomization to compare that to your dataset to see if your dataset is actually valuable, or if it contains a story or not
- [mentioned science paper](http://stat.wharton.upenn.edu/~buja/PAPERS/Wickham-Cook-Hofmann-Buja-IEEE-TransVizCompGraphics_2010-Graphical%20Inference%20for%20Infovis.pdf)
- see community notes for more details

__MY OPINION:__ :open_mouth:
  - showed advanced concepts I didn't totally follow
  - obviously knowledgeable, and was good to understand what she was after, but it was advanced enough so that it was a surface-level intro to a field I knew nothing about. Good to know it exists, then.

---

#### SVGs Beyond Mere Shapes
> Nadieh Bremer ([@NadiehBremer](https://twitter.com/@NadiehBremer))

- is data scientist and astronomer
- http://www.visualcinnamon.com/
- talk = explaning how to use SVG gradients in D3.js, and SVG filters, and how that works in her beautiful datavis experiments
  - [motion blur](http://tympanus.net/codrops/2015/04/08/motion-blur-effect-svg/), glow, gooey motion, blend modes (in CSS)

__MY OPINION:__ :blush:
  - the results of her experiments is really quite beautiful (good visual precendents for future projects :bulb:) but technically nothing special (I've done most of this myself already). Still, happy to be reminded of these possibilities.

---

#### Enhancing your maps and visualizations with WebGL GLSL Shaders
> Patricio Gonzalez Vivo ([@patriciogv](https://twitter.com/patriciogv))

- :eyes: [slides](http://patriciogonzalezvivo.github.io/openVis16/)
- works at [Mapzen](https://mapzen.com/) (all their tools are made opensource)
- :eyes: author of [The Book of Shaders](http://thebookofshaders.com/) :fire:
- he __LOVES__ shaders!
- used his Book of Shaders custom code editor to demo shader basics, its COOL :fire:
- Shaders on maps
  - :eyes: http://mapzen.com/tangram/play/
  - site let's you play with shaders in realtime on a map, cool stuff, visual editor is very friendly for beginners :fire:
- Example project of his: [Line Of Sight](http://patriciogonzalezvivo.github.io/LineOfSight/?type=visible#3/0.09/0.00)
  - https://github.com/patriciogonzalezvivo/LineOfSight
  - viz of satellites above the earth in realtime! :fire:
  - the method he used to encode the huge dataset of all satellite motion is using texture images where the RGB values store position data, and each pixel row is a satellite, etc..., then read with shaders (see Github link) :fire: :fire:
- A more concise example of encoding data into images, prepared for the conf :fire: :fire: :fire:
  - https://github.com/tangrams/WeatherOverTime

__MY OPINION:__ :heart_eyes:
  - amazing topic and tools
  - really bad accent (hard to understand)

---

#### Everything is Seasonal
> Zan Armstrong ([@zanstrong](https://twitter.com/zanstrong))

- whole talk = how when comparing data from different time periods, you must be __very very__ careful about comparing equivalent time spans (problems of leap days, etc.) and considering the context (seasonality, culture, nature of data, etc.)
- __very technical__ explanations of analysis that can be done on data to correct/adjust it, [see her github](https://github.com/zanarmstrong/everything-is-seasonal)
- see community notes for details

__MY OPINION:__ :open_mouth:
- very enthousiastic speaker, seems very competent with data math, too
- very very niche subject, but is applicable when we display timeseries data, good warning

---

#### Building Data Visualizations for Product
> Shirley Wu ([@sxywu](https://twitter.com/sxywu))

- works for Illumino, security firm, whole talk made actually talking to your client and figuring out their needs sound like amazing *__magic__* that no one had ever hear of (never heard of design school?)

__MY OPINION:__ :rage:
  - super boring, baby-level content, can't believe she got invited to speak. Sorry.

---

#### Animation, Pacing, and Exposition
> Tony Chu ([@tonyhschu](https://twitter.com/tonyhschu))

Quotes:
> "Graphic Design is the use of SPACE to control TIME." :fire:

> "I just blew your attention budget."

(in reaction to dumping too much info at once in front of the user)

- he's all about properly timing the presentation of bits of information to the user, not all at once, to explain an idea, step-by-step (sorta like 'scrolly-telling')
- :eyes: his famous work: [A Visual Introduction to Machine Learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)
- :eyes: another: [http://letsfreecongress.org/](http://letsfreecongress.org/)
- Explain your idea in small, easily assimilated chunks.
  - Goal: Exposition
  - Constraint: Attention
  - Tactics: Animation & Pacing
- it's all about how to __conserve this precious resource__ that is __attention__
- [slides](https://docs.google.com/presentation/d/1GOSyl4-iklcO0kIBFy-31zylaLC1R3uTwxX89bWt5D0/edit?usp=sharing)

__MY OPINION:__ :smile:
  - simple, clear talk about design principles for enabling focus, attention, explanation, in a world of too much data that is badly explained
  - inspiring

---

#### Informing Without Alienating
> Mona Chalabi ([MonaChalabi](https://twitter.com/MonaChalabi))

- Worked for 538 ([Dear Mona](http://fivethirtyeight.com/tag/dear-mona/)), now The Guardian
- Is about __"data journalism"__
- Started using [Instagram](https://www.instagram.com/mona_chalabi/) for sharing dataviz (hand-drawn images)
  - = great for seeing transparent debate, comments :fire:
- Principles:
  - Inclusivity: being inclusive with your data, making it understandable by the widest range of people
  - Responsibility/Honesty: representing the reality, knowing _**WHY**_ your data is how it is (bias, etc)
    - ex: a dataviz that shows the __uncertainty__ and __fallability__ of the data. [[1]](http://fivethirtyeight.com/features/how-we-are-forecasting-the-2016-presidential-primary-election/) [[2]](http://truth-and-beauty.net/projects/ukko)
  - Feeback: having open channels with your audience to check if your data is right

__MY OPINION:__ :neutral_face:
  - didn't learn much, but a little inspiring

---

#### Chartbuilder
> David Yanofsky ([@YAN0](https://twitter.com/YAN0))

- built an auto-D3-chart-building webapp called [Chartbuilder](https://github.com/Quartz/Chartbuilder), for Quartz
  - uses React and D3 (D4, actually)

__MY OPINION:__ :confused:
  - simple, funny guy, doesn't seem technically super proficient (playing it cool?) but the tool is cool for D3 noobs or journalists/reporters that don't know coding

---

#### 39 studies on human perception in 30 minutes
> Kennedy Elliott ([@kennelliott](https://twitter.com/kennelliott))

- is a perception researcher, works at Washington Post
- [her own recap on her presentation](https://medium.com/@kennelliott/39-studies-about-human-perception-in-30-minutes-4728f9e31a73#.4im7uyv21)
  - mentioned seminal perception study, at the root of all dataviz perception sutdies: Cleveland and McGill
  - that study's findings were proven by Heer and Bostock using Mechanical Turk :fire:
  - annotations skew the rememberence of a chart
  - pie charts more accurate than barcharts, supposedly (?!)

__MY OPINION:__ :blush:
  - useful as a theory recap
  - her pres was lightspeed and boring

---

#### Designing for Realtime Spacecraft Operations
> Rachel Binx ([@rachelbinx](https://twitter.com/rachelbinx))

Quotes:
> "Data visualization is not your creative outlet. Data visualization is making data understandable."


- worked at JPL on datavis; initially thought it would be a dream job, then came down to earth and did very simple datavis with very complicated data streams
- [great slides, 18 - 26](https://speakerdeck.com/binx/designing-for-spacecraft-operations?slide=18)
  - where datavis fits between design and art (it's much closer to design)
    - it can be placed anywhere in between, but probably:
      - projects for work are closer to design
      - project for fun are closer to art
  - design solves problems / art creates problems
- for JPL datavis, deliberately trying __NOT to tell a story__, create malleable tools to let users do their own exploration
- __lessons from working @ JPL__
  - know thy user
  - visualization literacy takes time
  - intuitive > shiny

__MY OPINION:__ :smile:
  - engaging, quirky speaker, fun to listen to
  - a good wake-up call to stay grounded, remember what design is all about

---

#### Reactive Building Blocks: Interactive Visualizations with Vega
> Arvind Satyanarayan ([@arvindsatya1](https://twitter.com/arvindsatya1))

- working on Vega with Jeff Heer, part of the University of Washington datavis clan
- whole talk is showing the differences between D3 and Vega's interaction handling
  - interaction model is better/faster/nicer to write in Vega
  - with it, you _declaratively_ define interactivity
  - Vega uses streams of events
  - easy to handle different signal types for desktop and mobile
  - [academic paper he wrote on this](http://idl.cs.washington.edu/files/2014-DeclarativeInteraction-UIST.pdf)
- examples:
  - [DimpVis](https://www.youtube.com/watch?v=DrLaYHzS9k8) by Christopher Collins @ UOIT
  - https://sandbox.github.io/demos/nba-shot-chart-vega/
- Links:
  - https://vega.github.io/vega-editor
  - http://vega.github.io/vega/

__MY OPINION:__ :blush:
  - Vega looks very cool, but hard to find a place for it in my process
  - looks promising for the future (not yet that useful, maybe)

---

#### Tiny Tools
> Adam Pearce ([@adamrpearce](https://twitter.com/adamrpearce))

- works at NYT, worked at Bloomberg before
- made many little D3 tools to work faster, reuse code, customize
- went thru all his code to find reusable bits and pieces, that's how he made his tools :fire:
  - :eyes: For _scrolly-telling_: https://github.com/1wheel/graph-scroll
  - :eyes: https://github.com/1wheel/d3-starterkit
    - :bulb: I could fork this and add my own snippets!
  - https://github.com/1wheel/swoopy-drag
- :eyes: [cool old-school aesthetic applied to graphs](http://www.bloomberg.com/graphics/year-ahead-2016/)
- :eyes: [other cool scrolling library by WSJ](https://github.com/WSJ/scroll-watcher)
- [slides](https://t.co/pMBrWWmG1I)

__MY OPINION:__ :blush:
  - good pres, useful content, practical

---

#### The Visual Uncertainty Experience
> Jessica Hullman ([@JessicaHullman](https://twitter.com/JessicaHullman))

- talk is about how we've displayed uncertainty in datavis, how we deal with probability statistics in datavis
- interesting: [Galton and regression towards the mean](http://blog.minitab.com/blog/statistics-and-quality-data-analysis/so-why-is-it-called-regression-anyway)

__MY OPINION:__ :neutral_face:
  - interesting topic, not so interesting talk

---

#### Untangling Tennis
> Kim Albrecht ([@kimay](https://twitter.com/kimay))

- talked about his [Untangling Tennis site](http://untangling-tennis.net/tool/)
- is into high-density data, high-res visualizations
  - his new work is about [Cosmic Web](http://cosmicweb.barabasilab.com/)

__MY OPINION:__ :neutral_face:
  - not so interesting, no take-aways

---

#### Our Planet Seen from Space
> Christine Waigl ([@chrys](https://twitter.com/chrys))

- all about using satellite imagery/data for tools & social causes
- there exists tons of __FREE__ satellite data!
  - should we care?
  - there's satellite imagery for:
    - education
    - social causes
    - history
    - etc...
  - data from:
    - [Sentinels](https://scihub.copernicus.eu/)
    - [Landsat/USGS](http://landsat.usgs.gov/Landsat_Search_and_Download.php)
    - [NASA Worldview](https://worldview.earthdata.nasa.gov/)
    - etc...
- examples
  - :eyes: http://projects.propublica.org/louisiana/

__MY OPINION:__ :blush:
  - very passionate about her field, interesting person, lives in Alaska to be closer to wildfire epidemic and help with social causes (?)

---

#### Finding What to Read: Visual Text Analytics Tools and Techniques to Guide Investigation
> Christopher Collins ([@ChrisNF](https://twitter.com/ChrisNF))

Quotes:
> "Datavis won't replace reading the books, but it can tell you which books to read."

- [is eminent datavis professor at UOIT, has research lab](http://vialab.science.uoit.ca/)
- are we suffering from _information overload_?
  - __NO__
  - we lack good exploration tools, personalized tools for each purpose
- complex projects he does with his students:
  - http://www.cs.toronto.edu/~jianzhao/webapp/FluxFlow/fluxflow.html
  - http://vialab.science.uoit.ca/wordsinpasswords/
  - :eyes: http://www.lexichrome.com/

__MY OPINION:__ :smile:
  - great academic resource, good work & ideas coming out of his lab
  - seems very smart and current on academic datavis world (as you might expect)

---

#### Designing Virtual Reality Data Visualizations
> Ana Asnes Becker ([@ana_becker](https://twitter.com/ana_becker))

- :eyes: young gun who made this [3D Nasdaq datavis](http://graphics.wsj.com/3d-nasdaq/)
  - datavis + 3D + VR = the next frontier? :fire:
  - she's not a technical person, she just had the idea
  - made with D3.js and Three.js, [here's how](http://www.storybench.org/how-to-make-a-simple-virtual-reality-data-visualization/)
  - that's almost all she talked about

__MY OPINION:__ :neutral_face:
  - interesting new idea
  - first talk ever, so not best quality but who cares, everyone's tired at this point
