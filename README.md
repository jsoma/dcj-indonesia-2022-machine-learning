Machine learning can mean a *lot* of different things. At its most basic, it can be described as "giving a computer some inputs and some outcomes, and letting the computer figure out the relationship between the two."

**Creating images**

* [DALL-E](https://openai.com/dall-e-2/)
* [Midjourney](https://www.midjourney.com/)

* [Vertex AI](https://cloud.google.com/vertex-ai)
* [Refinery](https://github.com/code-kern-ai/refinery)

## Finding outliers with Linear Regression

We know the outcome. Do we find some of those outcomes suspicious?

> Almost every single it's used in investigative reporting it's for school testing! [The AP did one about life expectancy](https://investigate.ai/ap-regression-unemployment/) but it's not very investigative and more similar to how we'll read logistic regression.

### Example: School Testing

[Cheating may be pervasive; Exclusive: TAKS surges raise questions about hundreds of schools](http://clipfile.org/?p=754), Dallas Morning News, 2004

[A PDF version with images](linear-regression-cheating-schools/TexasSchoolCheating.pdf)

* **Inputs:** Test scores in 3rd grade
* **Outputs:** Test scores in 4th grade
* **Relationship:** Low 3rd grade test scores usually means low 4th grade test scores

We're interested in **predicted outputs**.

## Finding bias with Logistic Regression

We know the outcome. Is something disproportionately affecting that outcome?

* [Reveal mortgage lending bias](https://investigate.ai/reveal-mortgages/)
* [Reuters asylum denials](https://investigate.ai/reuters-asylum/)

### Example: Speeding tickets

[Who gets a ticket, who gets a break?](http://archive.boston.com/globe/metro/packages/tickets/072003.shtml), Boston Globe, 2003

* **Inputs:** Car speed, gender, speed limit, in-town, race, etc...
* **Outputs:** Whether someone receives a ticket or a warning
* **Relationship:** Race and gender affect the outcome more than you'd expect

We're interested in **the relationship**.

## Letting a machine do the work with Classification

We label some of our data. Can a machine do the rest?

* [Buzzfeed spy planes](https://investigate.ai/buzzfeed-spy-planes/buzzfeed-surveillance-planes-random-forests/) 
* [LA Times crimes classifier](https://investigate.ai/latimes-crime-classification/using-a-classifier-to-find-misclassified-crimes/)

### Example 1: App reviews

[Apple says its App Store is ‘a safe and trusted place.’ We found 1,500 reports of unwanted sexual behavior on six apps, some targeting minors.](https://www.washingtonpost.com/technology/2019/11/22/apple-says-its-app-store-is-safe-trusted-place-we-found-reports-unwanted-sexual-behavior-six-apps-some-targeting-minors/), Washington Post, 2019

[How they did it](https://investigate.ai/wapo-app-reviews/predict-reviews/)

* **Inputs:** The words in the review
* **Outputs:** Whether the review is about unwanted sexual behavior
* **Relationship:** Words like "guy" and "pervert" imply it's about unwanted sexual behavior

We're interested in the **outputs**.

### Example 2: More app reviews!

[Hundreds of teletherapy app users report unresponsive therapists, unfair charges](https://juliaingram.github.io/therapy-apps/), Julia Ingram, class project, [code here](https://github.com/juliaingram/therapy-app-reviews)