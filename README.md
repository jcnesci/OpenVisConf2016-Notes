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

- whole talk = using \<canvas> to turn manipulate images (and their pixels), write image filters, export pixel data to do other stuff with (like mechanical knitting (not explained))
- she's written many small JS libraries to manipulate images
- :eyes: slides: http://kosamari.com/presentation/openvis-2016

:sunglasses: __MY OPINION:__
  - nice talk, knowledgeable about writing basic filters in the web and going between web/machines, interesting
  - I know she has given many other talks, perhaps some more focused on how to achieve the knitting thing, but this one seemed like a bit of a hodge-podge/collection of various little manipulations. That's not bad, but a little fragmented. Cool enough.

#### How To Simulate The Universe, In 134 Easy Steps 
> Nicky Case ([@ncasenmare](https://twitter.com/@ncasenmare))


- :eyes: [slides](http://ncase.me/OVC2016/)
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
  - Probability Simulations: see slides
  - Agent-Based Modeling: see slides

:wink: __MY OPINION:__
  - xxx

