# Anıl Bora | Personal Website

This repository contains the source code for my personal website. The website showcases my portfolio, courses, and contact information. The project is built using HTML, CSS, and Font Awesome for icons.

## Project Structure

```
  project/
  │
  ├── CSS/
  │ ├── global.css
  │ ├── main.css
  │ ├── tablet.css
  │ └── mobile.css
  ├── images/
  │ ├── anilbora.jpeg
  │ ├── python-course.jpg
  │ ├── data-science-course.jpg
  │ └── ai-courses.jpg
  ├── index.html
  └── README.md

```
  
## CSS Files

- **global.css**: Contains global styles shared across the entire site.
- **main.css**: Contains the main styles for the site.
- **tablet.css**: Styles specifically for tablet devices (max-width: 768px).
- **mobile.css**: Styles specifically for mobile devices (max-width: 500px).

## HTML Structure

### Head Section

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="keywords" content="personal, python, github, sql, sqlite">
    <meta name="description" content="Anıl Bora | Personal Web Site"> 
    <meta name="author" content="Anıl Bora">
    <meta name="robots" content="follow, index">
    <title>Anıl Bora | Personal Web Site</title>

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap" rel="stylesheet">

    <!-- Font Awesome -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />

    <!-- CSS -->
    <link rel="stylesheet" href="./CSS/global.css">
    <link rel="stylesheet" href="./CSS/main.css">
    <link rel="stylesheet" media="(max-width:768px)" href="./CSS/tablet.css">
    <link rel="stylesheet" media="(max-width:500px)" href="./CSS/mobile.css">
</head>
```
### Body Section
The body contains the following sections:

- Header: Navigation bar with links to different sections.
- Home: Main section with an image and personal information.
- Training: Information about different training modes.
- Courses: Detailed list of available courses with descriptions, instructor information, and ratings.
- Contact: Contact form to get in touch and social media links.
- Footer: Additional navigation to scroll back to the top.


## CSS Details
### Reset and Base Styles
```
/* Base CSS - Reset CSS */
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
a{
    text-decoration: none;
    color: #FFF;
}
html{
    font-family: "Open Sans", sans-serif;
}
```

### Header and Navbar Styles
```
/* Header - Navbar*/
header{
    position: sticky;
    top: 0;
    z-index: 999;
}
#navbar{
    color: #FFF;
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding: 0.5rem 0;
}
#navbar ul{
    list-style: none;
    display: flex;
    align-items: center;
}
#navbar ul li a{
    padding: 0.5rem;
}
#navbar ul li a:hover{
    background-color: #256ea1;
    border-radius: 0.3rem;
}
```

### Section Details
```
/* Home */
#home{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 2rem;
    border: 1px solid grey;
}
section#home img{
    max-width: 20%;
    height: auto;
    border-radius: 100%;
}
section#home p{
    opacity: 0.6;
    font-style: italic;
}
section#home h2{
    margin-top: 0.75rem;
}
```
### Training Section
```
/* Training */
#training{
    color: #FFF;
    padding: 1rem;
}
#training .items{
    display: flex;
    flex-direction: column;
}
#training .items .item{
    text-align: center;
    padding: 0.5rem;
    width: 100%;
}
#training .items .item:hover{
    color: #256ea1;
    background-color: #FFF;
    cursor: pointer;
    border-radius: 1rem;
}
```

### Courses Section
```
/* Courses */
#courses{
    color: #333;
    padding: 1rem;
}
.courses{
    display: flex;
    flex-direction: column;
    padding: 1rem;
}
.courses .course{
    display: flex;
    flex-direction: column;
    padding: 0.5rem;
    margin-bottom: 0.5rem;
}
.courses .course .course-img{
    margin-right: 0.5rem;
    position: relative;
}
.courses .course .course-img span{
    position: absolute;
    top: 1rem;
    left: 0;
    background-color: red;
    color: white;
    padding: 0.25rem;
    border-radius: 0.2rem;
}
.courses .course .course-info .title{
    letter-spacing: 0.1rem;
    font-weight: 700;
    margin-bottom: 0.25rem;
}
.courses .course .course-info .description{
    letter-spacing: 0.1rem;
    opacity: 0.7;
    margin-bottom: 0.25rem;
    text-align: justify;
}
.courses .course .course-info .instructor{
    font-size: 0.8rem;
    font-weight: 400;
    margin-bottom: 0.25rem;
}
.courses .course .course-info .rating{
    font-size: 0.7rem;
    opacity: 0.8;
    margin-bottom: 0.25rem;
}
```
### Contact Section
```
/* Contact CSS */
#contact{
    color: #FFF;
    padding: 1rem;
}
#contact .contact-form{
    max-width: 700px;
    margin: 0 auto;
    display: flex;
    flex-direction: column;
}
#contact .contact-form ul{
    list-style: none;
    display: flex;
    flex-direction: row;
    margin-top: 1rem;
    align-self: center;
}
#contact .contact-form ul li a{
    padding: 1rem;
    font-size: 2rem;
}
#contact .contact-form ul li a:hover{
    opacity: 0.6;
}
```

### Miscellaneous Styles
```
/* UP CSS */
a#up{
    width: 4rem;
    height: 4rem;
    border-radius: 4rem;
    background-color: #256ea1;
    color: white;
    text-align: center;
    position: fixed;
    bottom: 1rem;
    right: 1rem;
    display: flex;
    justify-content: center;
    align-items: center;
}
a#up i{
    font-size: 2rem;
}
a#up:hover{
    background-color: white;
    color: #256ea1;
    cursor: pointer;
    border: 1px solid #256ea1;
}

/* Color CSS */
.bg-dark-blue{
    background-color: #202e51;
}
.bg-light-blue{
    background-color: #256ea1;
}

/* Text CSS */
.heading-small{
    font-size: 1.25rem;
}
.heading-medium{
    font-size: 1.5rem;
}
.heading-big{
    font-size: 1.75rem;
}
.text-center{
    text-align: center;
}

/* Container */
.container{
    max-width: 1100px;
    margin: 0 auto;
}

/* Button CSS */
.btn{
    cursor: pointer;
    padding: 1rem 4rem;
    border-radius: 0.75rem;
    margin-top: 1.25rem;
}
.btn-primary{
    background-color: #256ea1;
}
.btn-primary:hover{
    background-color: #FFF;
    color: #256ea1;
    border: 1px solid #256ea1;
}
.btn-submit{
    background-color: forestgreen;
    border: none;
    font-size: 1.25rem;
    color: #FFF;
    transition: all 0.5s;
}
.btn-submit:hover{
    background-color: #FFF;
    color: forestgreen;
    border: 1px solid forestgreen;
}
.btn-block{
    width: 100%;
    text-align: center;
}

/* Form CSS */
.form-group{
    padding: 0.25rem 0;
}
.form-group label{
    display: block;
    margin-bottom: 0.25rem;
}
.form-control{
    width: 100%;
    resize: none;
    padding: 1rem;
    font-size: 1.25rem;
    border-radius: 0.5rem;
}
```

















