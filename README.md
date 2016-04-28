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

:eyes: : play.tensorflow.org (was an internal tool @ Google)

:smile: __MY OPINION:__
  - very good intro to ML for a beginner like myself, chains well with Kyle's talk afterwards (good conf planning)
  - no complaints about the talk; clear, concise, speakers are knowledgeable, not boring


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

:wink: __MY OPINION:__
  - not as crazy and fast as I expected, pretty well-spoken, not really structured, but fun
  - I feel like this was fun at the time, but not very memorable; maybe because his stream-of-consciousness style isn't necessarily super education/didactic
  - inspiring and showed me new things, but didn't "learn" too much


#### Drawing on \<canvas> - how computers read pixels
> Mariko Kosaka ([@kosamari](https://twitter.com/kosamari))

Quote:
> "knitting *__is__* coding" :fire:
(when talking about pushing & popping threads onto a crochet needle)

- [slides](http://kosamari.com/presentation/openvis-2016)
- whole talk = using \<canvas> to turn manipulate images (and their pixels), write image filters, export pixel data to do other stuff with (like mechanical knitting (not explained))
- she's written many small JS libraries to manipulate images

:sunglasses: __MY OPINION:__
  - nice talk, knowledgeable about writing basic filters in the web and going between web/machines, interesting
  - I know she has given many other talks, perhaps some more focused on how to achieve the knitting thing, but this one seemed like a bit of a hodge-podge/collection of various little manipulations. That's not bad, but a little fragmented. Cool enough.


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

:wink: __MY OPINION:__
  - good social motives to his use of datavis, interesting theoritical backbone to his material (on systems theory) which was high-level but also seemed quite knowledgeable about
  - didn't learn any techniques, per se, but some good examples and leads for building experiences with narrativity and visual explanations of complex systems


#### Do you know Nothing when you see it?
> Amelia McNamara

- is a statistics professor
- mentions a free book about randomization techniques
  - talk = using randomization to compare that to your dataset to see if your dataset is actually valuable, or if it contains a story or not
- [mentioned science paper](http://stat.wharton.upenn.edu/~buja/PAPERS/Wickham-Cook-Hofmann-Buja-IEEE-TransVizCompGraphics_2010-Graphical%20Inference%20for%20Infovis.pdf)
- see community notes for more details

:open_mouth: __MY OPINION:__
  - showed advanced concepts I didn't totally follow
  - obviously knowledgeable, and was good to understand what she was after, but it was advanced enough so that it was a surface-level intro to field I knew nothing about. Good to know it exists, then.

#### SVGs Beyond Mere Shapes 
> Nadieh Bremer ([@NadiehBremer](https://twitter.com/@NadiehBremer))

- is data scientist and astronomer
- http://www.visualcinnamon.com/
- talk = explaning how to use SVG gradients in D3.js, and SVG filters, and how that works in her beautiful datavis experiments
  - [motion blur](http://tympanus.net/codrops/2015/04/08/motion-blur-effect-svg/), glow, gooey motion, blend modes (in CSS)

:smirk: __MY OPINION:__
  - the results of her experiments is really quite beautiful (good visual precendents for future projects :bulb:) but technically nothing special (I've done most of this myself already). Still, happy to be reminded of these possibilities.


#### Enhancing your maps and visualizations with WebGL GLSL Shaders 
> Patricio Gonzalez Vivo

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

:heart_eyes: __MY OPINION:__
  - amazing.
  - really bad accent (hard to understand)


#### Everything is Seasonal 
> Zan Armstrong

- whole talk = how when comparing data from different time periods, you must be __very very__ careful about comparing equivalent time spans (problems of leap days, etc.) and considering the context (seasonality, culture, nature of data, etc.)
- __very technical__ explanations of analysis that can be done on data to correct/adjust it, [see her github](https://github.com/zanarmstrong/everything-is-seasonal)
- see community notes for details

:open_mouth: __MY OPINION:__
- very enthousiastic speaker, seems very competent with data math, too
- very very niche subject, but is applicable when we display timeseries data, good warning




