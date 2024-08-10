# Corby Conservation Union
## Introduction
#### Project Description
Project is to campaign, convey and provide insight on what Corby Conservation Union do, hence portray the importance of conservation of nature (green and animal conservation).
#### Project Purpose
The project is aimed at communicating with local, national and international audience the importance of conservation of our environment for future generation. This entails green and animal conservation, to reduce natural disaster experienced round the globe. Thus encourage every individual to play their part in any way they can.
The project provides several interactive features to enable users learn more about the organisation and easily navigate through the site to find desired content and support the organisation to continue conserving our ecosystem.
#### User Demographic
Initiative started from our local community Corby in Northamptonshire United  Kingdom, working with local communities, charities and community interest companies in and around Northamptonshire.  With a well thought after global initiative Corby Conservative Union is now engaging with other conservation entities around the globe. Other entities and individuals keen on  conservation of our planet natural resources and animals are encouraged to get involved through volunteering or material support for the organisations
## Design
#### Colour Scheme
The three main colours used are Granite Gray, Azure and Olive green. This is inline with the theme of this project "Go Green and animal conservation".
#### Topograhy
The Montserrat font is used  all through the website. Sans Serif is used as the backup font should for any reason the font isn't being imported into the site properly.
#### Imagery
The hero image is designed to aligned with the theme of the project showing outstanding green conservation surrounded by water and a house built with non-synthetic but  natural materials. Other images through the projects also focuses on green and animal  conservation.
## Features
The  core features/functionality of  this project is categorised as below. Features left unimplemented are also highlighted in this section.
### Existing Features
#### Navbar
A responsive navigation header where all the links to other html pages are embedded. Burger icon is used to indicate  navbar in mobile screens and landscape. For media screen 786px and up (tablets) navigation to other pages are indicated at the header. 
```html
 <header>
        <a href="index.html">
            <h1 id="logo">Corby Conservation Club</h1>
        </a>
        <input type="checkbox" name="nav-toggle" id="nav-toggle">
        <label for="nav-toggle" class="nav-toggle-label"><i class="fa-solid fa-bars-staggered"></i></label>
        <nav>
            <ul id="menu-card">
                <li><a href="index.html" class="active">Home</a></li>
                <li><a href="gallery.html">Gallery</a></li>
                <li><a href="register.html">Register</a></li>
                <li><a href="about-us.html">About Us</a></li>
                <li><a href="donate.html">Donate</a></li>
            </ul>
        </nav>
    </header
```
![Image showing the output of the program](./assets/images/readme-images/navbar.jpg). ![Image showing the output of the program 768px and above](./assets/images/readme-images/navbar%20tablets.jpg)
#### Footer and Social Media Icons
A responsive footer is included for user interaction and where they can follow Corby Conservation Union social network. A home page for Facebook, Instagram, Twitter(X) and YouTube is embedded through the social media icons.
```html
 <footer>
        <h2 id="networks">Follow us</h2>
        <ul id="network-with-us">
            <li><a href="https://www.facebook.com/" target="_blank" rel="noopener"
                    aria-label="Visit us on facebook (open in a new tab)"><i class="fa-brands fa-facebook"></i></a></li>
            <li><a href="https://x.com/" target="_blank" rel="noopener"
                    aria-label="Visit us on X (open in a new tab)"><i class="fa-brands fa-x-twitter"></i></a></li>
            <li><a href="https://www.instagram.com/" target="_blank" rel="noopener"
                    aria-label="Visit us on instagram (open in a new tab)"><i
                        class="fa-brands fa-square-instagram"></i></a></li>
            <li><a href="https://www.youtube.com/" target="_blank" rel="noopener"
                    aria-label="Visit us on youtube (open in a new tab)"><i class="fa-brands fa-youtube"></i></a></li>
            <li><a href="https://www.linkedin.com/" target="_blank" rel="noopener"
                    aria-label="Visit us on linkedin (open in a new tab)"><i class="fa-brands fa-linkedin"></i></a></li>
        </ul>
    </footer>
```
![Image showing the output of the program](./assets/images/readme-images/footer-mobile-screen.jpg)
#### Buttons and Links
Responsive button and links were used. “Get Involved” button in registration page is linked to https://formdump.codeinstitute.net. “Donate” button on donate page is linked to thank-you.html. The icons buttons to social media are all linked to home page of respective social network.
```html
<div>
    <button type="submit" class="donate-button">Donate</button>
</div>
```
```html
<div>
    <button type="submit" class="join-button">Get Involved!</button>
</div>
```
![Image showing the output of the program](./assets/images/readme-images/donate-button.jpg). ![Image showing the output of the program](./assets/images/readme-images/get-involved-button.jpg).
#### Image Gallery
Image Gallery is a page dedicated to green and animal conservation images compiled with Masonry redesign style with column counts for different screen sizes. "alt" attribute included to describe the images and enable screen reader to read out the description of the image for visually impaired users.
```html
<section id="gallery">
    <h2 class="hidden-heading">Gallery</h2>
    <div id="pictures">
        <img src="assets/images/peng.jpg" alt="Adélie Penguin getting close extinction">
        <img src="assets/images/green-peace.jpg" alt="Our team on green peace day">
        <img src="assets/images/hippo.jpg" alt="African hippo">
        <img src="assets/images/ccu-plastic.jpg" alt="Sanitizing our rivers">
        <img src="assets/images/cuu-nature.jpg" alt="Nature">
        <img src="assets/images/ccu-river.jpg" alt="Sanitizing our local rivers of plastic">
        <img src="assets/images/ourpeople.jpg" alt="Our people ready for animal rescue">
        <img src="assets/images/zeb.jpg" alt="African zebra">
        <img src="assets/images/waterfall.jpg" alt="Corby Conservation union on safari waterfall">
        <img src="assets/images/splash.jpg" alt="Corby Conservation union brought cave of ggod hope south Africa back to life">
    </div>
</section>
```
![Image showing the output of the program](./assets/images/readme-images/gallery-page.jpg).
#### Register Form
Responsive registration form created to accept First name, Last Name, Email address and radio button to select label options. It is expected that any none text input on email address, first and last name will through up an error message. Users are also restricted to select only one label. 
```html
<form id="registration-form" action="https://formdump.codeinstitute.net" method="POST">
    <h2>Register with us!<i class="fa-solid fa-handshake"></i></h2>
    <br>
    <label for="first-name">First Name</label>
    <input type="text" name="first_name" id="first-name" class="text-input" autocomplete="on" required>
    <br>
    <label for="last-name">Last Name</label>
    <input type="text" name="last_name" id="last-name" class="text-input" required>
    <br>
    <label for="email-address">Email Address</label>
    <input type="email" name="email_address" id="email-address" class="text-input" required>
    <div class="radio-buttons">
        <div>
            <label for="wildlife">Wildlife</label>
            <input type="radio" name="conservation_preference" id="wildlife" value="wildlife" required checked>
        </div>
        <div>
            <label for="go-green">Go Green</label>
            <input type="radio" name="conservation_preference" id="go-green" value="go-green" required>
        </div>
        <div>
            <label for="both">Both</label>
            <input type="radio" name="conservation_preference" id="both" value="both" required>
        </div>
    </div>
    <div>
        <button type="submit" class="join-button">Get Involved!</button>
    </div>
</form>
```
![Image showing the output of the program](./assets/images/readme-images/registration-form.jpg).
#### Donate Form
Responsive donate form designed to accept Name on Card, 16 digits card number , card expiry date, 3 digits CVC card number and amount. This section is design for alpha numeric input, however  specific conditions must be met before the form can submit. Name on Card must be alpha, card number must be numeric and can’t input more than 16 digits. Expiry date must be a future date, CVC must be numeric and can’t exceed 3 digits and amount must be numeric.
```html
<div id="donate">
                <form id="donation-form" action="thank-you.html" method="GET">
                    <h2>Support Us<i class="fa-solid fa-circle-dollar-to-slot"></i></h2>
                    <br>
                    <h3 class="phrase">"It's not too late to Go Green and save wildlife, but we must act together".</h3>
                    <br>
                    <div>
                        <label for="name-on-card">Name on Card</label>
                        <input type="text" name="name_on_card" id="name-on-card" class="text-input" required>
                    </div>
                    <div>
                        <label for="card-number">Card Number</label>
                        <input type="text" inputmode="numeric" pattern="[0-9\s]{13,16}" autocomplete="cc-number"
                            name="card_number" id="card-number" class="number-input" placeholder="xxxx xxxx xxxx xxxx"
                            maxlength="16" required>
                    </div>
                    <br>
                    <div>
                        <label for="expiry-date">Expiry Date</label>
                        <input type="date" name="expiry_date" id="expiry-date" class="date-input" value="2024-08-09"
                            required>
                    </div>
                    <br>
                    <div>
                        <label for="cvc">CVC</label>
                        <input type="text" inputmode="numeric" pattern="[0-9]{3}" autocomplete="cc-number"
                            name="cvc_number" id="cvc" class="number-input" maxlength="3" placeholder="xxx" required>
                    </div>
                    <br>
                    <div>
                        <label for="amount">Amount</label>
                        <input type="number" name="amount_number" id="amount" class="number-input" value="0.00"
                            required>
                    </div>
                    <div>
                        <button type="submit" class="donate-button">Donate</button>
                    </div>
                </form>
            </div>
```
![Image showing the output of the program](./assets/images/readme-images/donate-page.jpg)
#### Improvement Features
* Donate button can be linked to banks via financial services network like visa, master card etc.
* Videos, iframe or pictures functionalities that illustrates green and wildlife conservation  can be added to gallery.html file
* News feed can be added to present news specifically targeted to green and wildlife conservation, including any announcement from Corby Conservation Union.
## Manual Testing
### Quality Assurance
### User Experience Assurance
### Features Testing
#### Lighthouse Perfomance
#### Validation Testing
#### Browser compatibility
#### Screen sizes Responsiveness
#### Accessibility
#### Bugs Resolved
#### Bugs Unresolved
## Deployment
The project was deployed to GitHub Pages using the following steps..
1.	Log in to GitHub and locate my repository <https://github.com/Cutbert1/Corby-Conservation-Club> 
2.	At the top of the Repository (not top of page), locate the **Settings** Button on the menu.
3.	Scroll down the Settings until you locate the **Pages**, then click.
4.	In the **Build and Deployment**, select **main branch** and ensure the folder is set to **root folder** and click **save**
5.	Return to code tab of GitHub repo. Delay for few minutes to enable the build finish, then refresh  the page. 
6.	Check deployment section on the code page (right hand side bar)
7.	Click **github-pages** to see the live URL

## Credits
### Codes
### Tutorials
### Photos
### Text Content