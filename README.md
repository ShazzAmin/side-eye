Side Eye
========

*by Shazz Amin, Gordon Guan, Ellen Huang, Mivia Li*

*for **Hack the North 2018***

Intuitive and seamless navigation for multi-monitor setups.

## Project Submission

### Inspiration
Multi-monitor setups are now commonplace, increasing productivity by providing not only more space, but an extra organizational layer for managing tasks. However, with the complexity we gain through more organization we lose simplicity. With the desktop originally designed for being able to comprehend the current state of the system in a single glance, we should be able to use modern technology as a way to bridge the gap and make human interface more intuitive.

### What it does
Side Eye uses facial cues captured by consumer webcams in order to assist with one concept made more complicated by multi-display technologies: navigation.

### How we built it
Side Eye uses OpenCV to keep a running model of the user's facial state, capturing relevant features and detecting gesture events. With a machine learning layer, these features are mapped to a list of actions, designed to make the experience of using multiple monitors seamless and intuitive.

### Challenges we ran into
Some challenges we ran into included consolidating the compatibility of several components we used to create the project. Problematically, one of the key components we used for eye tracking was written in C++ while the rest of the codebase was in Python - in the interest of time constraints and ease-of-implementation we decided to translate our code into C++ to accommodate that dependency. Some effort was also required to adapt the code from a proof-of-concept demonstration application to a library-like include that would generate data in the format required by our machine learning layer.

### Accomplishments that we're proud of
One thing we're proud of was our initial planning and scoping for our project idea. We were able to create an accurate plan-of-action and divide up the work in an effective way which allowed us to complete the project efficiently and without major hassles.

### What we learned
In the development of Side Eye, we learned a lot about using the inter-connectivity of many independent technologies. In order for our final product to function, we combined several libraries and frameworks (OpenCV, Qt, etc.) that were incompatible in several way. We learned about conceding to the "good solution" and instead embracing the "practical solution", in order to create a final working solution.

### What's next for Side Eye
For the future of Side Eye, several more independent gestures and features such as "wink-to-select" and gesture based window switching may be added to capitalize more on the usage of facial cues for navigation.

### Built With
* OpenCV
* Qt
* Machine learning
