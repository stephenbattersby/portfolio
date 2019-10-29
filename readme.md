### How to maintain this website

The web pages are built with vanilla HTML and CSS and is easy to update and maintain. HTML - is merely a mark-up language and using a few HTML tags should help update the copy.

## Meta-data (head)
```
    <meta charset="utf-8">
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Stephen Battersby Science Writer & Editor</title>
    <link rel="stylesheet" href="css/style.css">
    <script src="https://kit.fontawesome.com/ec796bd4f8.js"></script>
    <link href="https://fonts.googleapis.com/css?family=Nunito&display=swap" rel="stylesheet">
    <link rel=“stylesheet” href=“https://cdnjs.cloudflare.com/ajax/libs/bulma/0.7.2/css/bulma.css“> 
</head> 
```

To change the title type within the ```title`` tag - note tags must be opened and closed ```<title></title>``
CSS will be dealt with in a separate section - the file path is in the meta-data
Fontawesome is the free library that has been used for icons - icons may be added and removed but this meta-data must stay here for the icons to display
Font meta is the google font used - Nunito - a sans serif type

## Header section not to be confused with the metadata in head

1. Changing text in the hero section or header - the only text here is the text in text tags. This is not the head which is purely meta-data, in this section you have both text and images.

```<h1><h1>``` to ```<h6></h6>``` tags contain all the headings of different sizes - h1 the most important and h6 the least important for search engines 

2. Changing the image - the image is in the assets folder ```assets/stephen-battersby-photos/stephen-battersby-science-writer-editor.png``` this is the relative path - use a .png format and replace the photo with the same file-path and name so that it is meta-tagged. This will auto-update the image

3. Updating the CV - as with the CV the file needs to overwrite the existing file in file-path ```assets/stephen-battersby-science-writer-editor- web-cv.pdf``` and the CV will auto-update

```
<header class="hero-section" id="hero-section">
            <div class="card-1">
                    <div class="hero-image">
                            <img name="stephen-battersby-science-writer" class="profile-image"
                            src="assets/stephen-battersby-photos/stephen-battersby-science-writer-editor.png"
                            alt="Stephen Battersby Science Writer" />
                            </div>     
        </div>
            <div class="hero-text">                           
                <h1>Stephen Battersby </h1>
                <h1>Science writer & editor</h1>
                <div class="contact-details">
                <h1>
                    <a target="_blank"
                    href="assets/stephen-battersby-science-writer-editor- web-cv.pdf">
                        CV </a>
                    </h1>
                    <h1>
                    <a target="_blank" 
                    href="https://www.linkedin.com/in/stephen-battersby-84a81526/">
               LinkedIn</a>
            </h1>
            <h1> 
                <a target="_self" 
                href="mailto:stephenbattersby@gmail.com">
                <i class="fas fa-envelope"></i></a>
            </h1>
            </div>
            </div>
        </header>
```
## The bio and client list section

Updating the text:

1. All text is in paragraph tags ```<p></p>``` update text make sure the tags are opened and closed
2. The ```<em></em>``` or emphasis tags are used for Nature and New Scientist. These tags also need to be closed.
3. Do not remove the ```<hr>``` self-closing tag between the client list and main bio - the page layout will break, the tag is a horizontal (invisible line) between the two sections.
4. The words client list are in ```<h4></h4>```tags while the actual clients are a list of names in ```<li></li>``` tags, if clients need to be added or removed update the names within the tags and make sure they are opened and closed.
5. Make sure the ```<div></div>``` tags or division tags are not removed, this will also change the styling.

```
        <section class="bio-display">
            <div class="bio-text">
                <p>I edit high-level reports for government and business. That means plunging deep into
                    a technical topic and untangling expert copy to create a compelling read with a clear message.
                    I also write popular science articles, and set questions for University Challenge. </p>

                <p>After a little astrophysics research I was an editor at <em>Nature</em> and
                    then <em>New Scientist</em>. before going freelance to write about black holes,
                    icy moons and the end of time. </p>
            </div>
            <hr>
            <div class="client-list">
                <div>
                    <h4>CLIENT LIST</h4>
                </div>
                <ul class="clients-caption"></ul>
                <li>Government Office for Science</li>
                <li>New Scientist</li>
                <li>Proceedings of the National Academy of Sciences</li>
                <li>University of Birmingham</li>
                <li>Xyntéo</li>
                <li>M Squared Lasers</li>
                <li>Innovate UK</li>
                <li>Engineering and Physical Sciences Research Council</li>
                <li>DNV-GL</li>
                <li>Snam S.p.A.</li>
                <li>UK Quantum Technology Hub for Sensors and Metrology</li>
                <li>University Challenge</li>
            </div>
        </section>
```
## The bio and client list section

1. Changing images - once again the images file path are in the assets folders cover-images-for-editing and cover-images-for-writing.
2. Select the picture and save it in their respective folders.
3. change the image name attribute within the inverted commas ```name="uk-govt-cover-quantum-technologies"``` update the src or source attribute ```src="assets/cover-images-for-editing/futuristic-chado-nihi-pixabay.jpg"``` with the file path within the inverted commas and update the alt tag within the inverted commas ```alt="quantum-technologies-photo" ```
Make sure the image tag ```<img``` opens before the name, src, alt attributes, the equal sign does not disappear and that the text is within inverted commas once you have updated it, the image tag closes after the attributes ```/>```

4. Changing text - text is in ```<h5></h5> tags 
5. Chaning links - the links are nested in an anchor tag ```<a target="_blank"``` leave this section as it is as it opens the link in a new page. Update the ```href``` make sure that the a tag is closed```>``` this tag is particularly easy to miss as it comes after the inverted commas but BEFORE the h5 text!
The anchor tag closes AFTER the text ```</a>```
```
<img name="uk-govt-cover-quantum-technologies" class="portfolio-photo"
                        src="assets/cover-images-for-editing/futuristic-chado-nihi-pixabay.jpg"
                        alt="quantum-technologies-photo" />
                    <h5>
                        <a target="_blank"
                            href="https://www.gov.uk/government/publications/quantum-technologies-blackett-review">
                            Quantum technologies - a Blackett Review for the UK government
                           </a>
                    </h5>
```

## Changing styling - a note about the styling of this app
Mainly uses vanilla CSS with Flexbox and Grid - be careful not to touch any of the meta-data in the html which refer to css class ``` <div class="client-list">``` 

The CSS is in a separate file and contains mainly the colors, font sizes, margins and padding. You may want to change the hero background image which is in the CSS section - once again replace the image in the folder without chaning the name or extension (jpg). It should auto update. If you change the file type to png or svg then change the extension!
```
.hero-section {
	display: flex;
	background: url("/assets/banner-hero.jpg");
	background-size: cover;
	background-repeat: no-repeat;
	opacity: 0.9;
	background-color: rgb(178, 182, 185);
}
```

Save files and send the GitHub link with updates.

Publishing directly to the web with GH Pages
Make your changes check that you are happy with them with live server
Right click on the html page and open the page with live server
Once you are happy save the changes and then push them live with the commands

git add.
git commit -m"your notes about the change"
git push

