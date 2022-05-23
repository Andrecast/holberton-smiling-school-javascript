# 0x0F. Build a web app in JavaScript

In this project, you will finalize the previous project  [0x0B. Implement a design with bootstrap](https://intranet.hbtn.io/rltoken/oiPG7fxT8IPuYTMm8gbVBw "0x0B. Implement a design with bootstrap")  and make some parts dynamic with Javascript (JQuery exactly).

You will reuse final files of  [0x0B. Implement a design with bootstrap](https://intranet.hbtn.io/rltoken/oiPG7fxT8IPuYTMm8gbVBw "0x0B. Implement a design with bootstrap")  and update them.

You will use all HTML/CSS/Accessibility/Responsive design/Bootstrap/Javascript knowledges that you learned previously.

You won’t have a lot of instruction, you are free to implement it the way that you want - the objective is simple: Have fully functional web pages that look the same as the designer file.

Here the final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/3/3c71cc99d2fc1c12a3d3.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220523%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220523T215111Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=da9eb38d990335fce0862118a7b5c041f4a21959f2703a6b023dd425977a9f59)

This webpage has been designed by Nicolas Philippot, UI/UX designer. You can find final screens  [here](https://intranet-projects-files.s3.amazonaws.com/holbertonschool-webstack/623/Archive.zip "here")

### Requirements

-   You have to use Bootstrap
-   Your  `styles.css`  must be as small as you can -  **you must use as much as you can Bootstrap classes**
-   You have to use JQuery
-   Your  `scripts.js`  must contain all your Javascript part
-   Your Javascript must be executed only when the document is loaded

### Imports

For this project, you will need: fonts from Google, JQuery, Bootstrap CSS/JS

```
<link href="https://fonts.googleapis.com/css?family=Source+Sans+Pro&display=swap" rel="stylesheet">
<link href="https://fonts.googleapis.com/css?family=Coiny&display=swap" rel="stylesheet">

<script src="https://code.jquery.com/jquery-3.4.1.min.js" integrity="sha256-CSXorXvZcTkaix6Yvo6HppcZGetbYMGWSFlBw8HfCJo=" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/js/bootstrap.min.js" integrity="sha384-wfSDF2E50Y2D1uUdj0O3uMBJnjuUD4Ih7YwaYd1iqfktj0Uod8GCExl3Og8ifwB6" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js" integrity="sha384-ApNbgh9B+Y1QKtv3Rn7W3mgPxhU9K/ScQsAP7hUibX39j7fakFPskvXusvfa0b4Q" crossorigin="anonymous"></script>

<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.4.1/css/bootstrap.min.css" integrity="sha384-Vkoo8x4CGsO3+Hhxv8T/Q5PaXtkKtu6ug5TOeNV6gBiFeWPGFN9MuhOf23Q9Ifjh" crossorigin="anonymous">

<link rel="stylesheet" href="styles.css">
<script src="scripts.js"></script>

```

## Tasks

### 0. Reuse and polish your Bootstrap integration

mandatory

Score:  0.00%  (Checks completed: 0.00%)

Copy files from  [0x0B. Implement a design with bootstrap](https://intranet.hbtn.io/rltoken/oiPG7fxT8IPuYTMm8gbVBw "0x0B. Implement a design with bootstrap"):

-   `homepage.html`  ->  `0-homepage.html`
-   `pricing.html`  ->  `0-pricing.html`
-   `courses.html`  ->  `0-courses.html`
-   `styles.css`  and any files/folders needed (images, fonts…)

And finalize the design if it’s not done yet - the final result should be the same as these screens:

-   [Homepage](https://intranet.hbtn.io/rltoken/X5mp-bZwa8Jzi3HI4xqSLA "Homepage")  -  [fig file](https://intranet.hbtn.io/rltoken/zsIWYdFMnWtImWisjLgfTw "fig file")
-   [Pricing](https://intranet.hbtn.io/rltoken/Bbop8wwZOLJsavfT6szqdQ "Pricing")  -  [fig file](https://intranet.hbtn.io/rltoken/5yAyDbQvLAVmm3IC_NRV3g "fig file")
-   [Courses](https://intranet.hbtn.io/rltoken/PSFYeol4NYMEmSBsxUyuoQ "Courses")  -  [fig file](https://intranet.hbtn.io/rltoken/Jzp3WS1dZwYd8Q_wTIYp9Q "fig file")

Important notes with Figma:

-   if your computer doesn’t have missing fonts, you can find them here:  [source-sans-pro](https://intranet.hbtn.io/rltoken/Ei8qgkDzThkeVZMZYZydHg "source-sans-pro")  and  [Spin-Cycle-OT](https://intranet.hbtn.io/rltoken/SZKEX6sWitAn-vK8bZLvhA "Spin-Cycle-OT")
-   some values are in float - feel free to round them
-   “Be pixel perfect” - yes! but mainly make sure colors, size and position are correct.  #C271FF  is not  purple.

For this task, please write an amazing  `README.md`

**Interactions note:**

-   Web pages must switch to the tablet version when the screen width is 768px
-   Web pages must switch to the mobile version when the screen width is 576px
-   button hover/active:  `opacity: 0.9`

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `0-homepage.html, 0-pricing.html, 0-courses.html, styles.css, README.md`

Done!  Help  QA Review

### 1. Homepage - quotes

mandatory

Score:  0.00%  (Checks completed: 0.00%)

From  `0-homepage.html`, create  `1-homepage.html`.

Replace static quotes by dynamic loading:

-   URL:  `https://smileschool-api.hbtn.info/quotes`
-   No static quotes should be present in the quotes section
-   During the Ajax request, a loader should be present
-   Carousel should work like before

Example of my loader:

```
HTML:
<div class="loader"></div>

CSS:
.loader {
    border: 10px solid #f3f3f3;
    border-top: 10px solid #C271FF;
    border-radius: 50%;
    width: 80px;
    height: 80px;
    animation: spin 2s linear infinite;
    margin: auto;
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

```

Final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/044058b378bfef994b7c9dd672de1dca33d5f576.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220523%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220523T215111Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=950237ef3aae8a54a0dfb1feed91555fdea0cb28e9c989e90175775afe9c4de1)

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `1-homepage.html`

Done!  Help  QA Review

### 2. Homepage - popular tutorials

mandatory

Score:  0.00%  (Checks completed: 0.00%)

From  `1-homepage.html`, create  `2-homepage.html`.

Replace static video cards by dynamic loading:

-   URL:  `https://smileschool-api.hbtn.info/popular-tutorials`
-   No static video cards should be present in the section
-   During the Ajax request, a loader should be present
-   Carousel should work by sliding card by card (like GIF below) - this kind of carousel is not unique, make it generic to reuse it easily!
-   Don’t forget the responsive part!

Final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/0efb5ff68c622f830a70e7aaf16bac87822462af.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220523%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220523T215111Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=00b8d9b6476ab5e259f1b5479091c56cbe2bae991a94ce1fb12d347148bdbaec)

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `2-homepage.html`

Done!  Help  QA Review

### 3. Homepage - latest videos

mandatory

Score:  0.00%  (Checks completed: 0.00%)

From  `2-homepage.html`, create  `homepage.html`.

Replace static video card by dynamic loading:

-   URL:  `https://smileschool-api.hbtn.info/latest-videos`
-   No static video cards should be present in the section
-   During the Ajax request, a loader should be present
-   Carousel should work by sliding card by card (like GIF below) - this kind of carousel is not unique, make it generic to reuse it easily!
-   Don’t forget the responsive part!

Final result:

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/c9a421edef604cee434f02f26328f6a549abd81a.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220523%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220523T215111Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5e929ccc320e9fa3b22ef593bcefac968dac41efd100932aaa87c36e40b48231)

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `homepage.html`

Done!  Help  QA Review

### 4. Pricing - quotes

mandatory

Score:  0.00%  (Checks completed: 0.00%)

From  `0-pricing.html`, create  `pricing.html`.

Replace static quotes by dynamic loading:

-   URL:  `https://smileschool-api.hbtn.info/quotes`
-   No static quotes should be present in the quotes section
-   During the Ajax request, a loader should be present
-   Carousel should work like before

Same as the  `homepage.html`

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `pricing.html`

Done!  Help  QA Review

### 5. Courses

mandatory

Score:  0.00%  (Checks completed: 0.00%)

From  `0-courses.html`, create  `courses.html`.

Replace static video card by dynamic loading:

-   URL:  `https://smileschool-api.hbtn.info/courses`
    -   `GET`  parameters:
        -   `q`: search value (in our case, the value of the field KEYWORDS)
        -   `topic`: topic filter value (in our case, the value of the field TOPICS)
        -   `sort`: order of all courses (in our case, the value of the field SORT BY)
-   No static video cards should be present in the section
-   During the Ajax request, a loader should be present
-   Dropdowns are dynamic (coming from the API):
    -   Topic: list of  `topics`
    -   Sort by: list of  `sorts`
-   Search value should be initialized by the value  `q`  in the API response
-   The list of video cards is coming from  `courses`  in the API response
-   API request must be done when:
    -   Search value is changing
    -   A new Topic is selected
    -   A new Sort by is selected

![](https://holbertonintranet.s3.amazonaws.com/uploads/medias/2020/4/b081f3358ab5e79f44afc847d882bcf6fd5ef517.gif?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOU5BHMTQX4%2F20220523%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20220523T215111Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=cbc11f1aa43367ba9779fc9e58b1d1ea55d3d52840bf1c096711fe9fdb5c344d)

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `courses.html`

Done!  Help  QA Review

### 6. JSON to XML

#advanced

Score:  0.00%  (Checks completed: 0.00%)

Convert all your JSON Ajax call to another API… a XML API!

Copy files - same content, except loading  `xml-scripts.js`  instead of  `script.js`

-   `homepage.html`  ->  `xml-homepage.html`
-   `pricing.html`  ->  `xml-pricing.html`
-   `courses.html`  ->  `xml-courses.html`

And use this API:

-   quotes:  `https://smileschool-api.hbtn.info/xml/quotes`
-   popular tutorials:  `https://smileschool-api.hbtn.info/xml/popular-tutorials`
-   latest videos:  `https://smileschool-api.hbtn.info/xml/latest-videos`
-   courses:  `https://smileschool-api.hbtn.info/xml/courses`

Final result should be the same as the JSON API version

**Repo:**

-   GitHub repository:  `holberton-smiling-school-javascript`
-   File:  `xml-scripts.js, xml-homepage.html, xml-pricing.html, xml-courses.html`

