### 1. If we use a p tag and set background of it like yellow. then it is taking whole line why?

> P tag is a block element and it takes all available space.

---

### 2. How to add favicon in html?

```html
<!-- set favicon icon  -->
<link rel=" icon" href="favicon.ico" type="image/x-icon" />
```

---

### Clone Website - [Linux Torwald Portfolio]("codehelp-linus-torvalds-tribute.netlify.app")

![Linux Torwald Portfolio](/01%20-%20HTML%20Basics/02%20-%20HTML%20Basics/tribute%20hw.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tribute - Linus Torwalds</title>
  </head>
  <body>
    <h1>Linus Torvalds</h1>
    <p>The Creator of Linux</p>
    <figure>
      <img
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/e8/Lc3_2018_%28263682303%29_%28cropped%29.jpeg/220px-Lc3_2018_%28263682303%29_%28cropped%29.jpeg"
        alt="Linus Torvalds"
      />
      <figcaption>A photograph of Linus Torvalds</figcaption>
    </figure>
    <h2>Biography</h2>
    <p>
      Linus Torvalds is a Finnish-American software engineer who is the creator
      and principal developer of the Linux kernel, which is the kernel for a
      number of operating systems. He also created the version control system
      Git. Torvalds was born on December 28, 1969 in Helsinki, Finland. He
      studied computer science at the University of Helsinki, and he developed
      the Linux kernel as a student project in 1991. Since then, the Linux
      kernel has become one of the most widely used kernels in the world,
      powering everything from smartphones to supercomputers.
    </p>
    <h2>Achievements</h2>
    <ul>
      <li>
        1991 - Created the Linux kernel and the version control system Git
      </li>
      <li>
        2004 - Named one of the "100 Most Influential People in the World" by
        Time magazine in 2004
      </li>
      <li>
        2010 - Received an honorary doctorate from the University of Helsinki in
        2010
      </li>
      <li>
        2010 - Received the 2010 Millennium Technology Prize and the 2012 Free
        Software Foundation's Award for the Advancement of Free Software
      </li>
      <li>
        2013 - Inducted into the Internet Hall of Fame in 2013 for his
        contributions to the development of the Linux kernel and the creation of
        Git
      </li>
      <li>
        2014 - Inducted into the Hall of Fame of the Computer History Museum in
        2014
      </li>
      <li>
        2015 - Received the 2015 IEEE Computer Society Computer Pioneer Award
      </li>
      <li>2019 - Received the 2019 ACM SIGOPS Hall of Fame Award</li>
      <li>
        2021 - Awarded the Takeda Foundation's 2021 Takeda Award for Social
        Contribution, which recognizes individuals who have made significant
        contributions to society through technology
      </li>
      <li>
        2021 - Received the 2021 IEEE Masaru Ibuka Consumer Electronics Award,
        which recognizes individuals who have made significant contributions to
        the field of consumer electronics
      </li>
    </ul>
    <blockquote>
      <p>"One of the most influential people in the world."</p>
      <cite>
        -- Time Magazine
        <a
          href="http://www.thefamouspeople.com/profiles/linus-torvalds-3972.php"
        >
          The Famous People
        </a>
      </cite>
    </blockquote>
    <h2>Resources</h2>
    <p>Learn more about Linus Torvalds and his work:</p>
    <ul>
      <li>
        <a href="https://en.wikipedia.org/wiki/Linus_Torvalds">
          Wikipedia page on Linus Torvalds</a
        >
      </li>
      <li>
        <a href="https://www.linustorvalds.com/">
          Linus Torvalds's personal website</a
        >
      </li>
      <li><a href="https://www.kernel.org/"> The Linux Kernel Archives</a></li>
    </ul>
  </body>
</html>
```

---

### Clone a picture of table

![Table Home Work](/01%20-%20HTML%20Basics/02%20-%20HTML%20Basics/table%20hw.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <style>
      table,
      th,
      tr,
      td {
        border: 1px solid black;
      }
    </style>
  </head>
  <body>
    <table>
      <thead>
        <tr>
          <th rowspan="3">Day</th>
          <th colspan="3">Seminar</th>
        </tr>
        <tr>
          <th colspan="2">Schedule</th>
          <th rowspan="2">Topic</th>
        </tr>

        <tr>
          <th>Begin</th>
          <th>End</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td rowspan="2">Monday</td>
          <td rowspan="2">8:00 a.m.</td>
          <td rowspan="2">5:00 p.m.</td>
          <td>Introduction to XML</td>
        </tr>
        <tr>
          <td>Validity: DTD and Relax NG</td>
        </tr>
        <tr>
          <td rowspan="4">Tuesday</td>
          <td>8.00 a.m.</td>
          <td>11.00 a.m.</td>
          <td rowspan="2">Xpath</td>
        </tr>

        <tr>
          <td rowspan="2">11.00 a.m.</td>
          <td rowspan="2">2.00 p.m.</td>
        </tr>
        <tr>
          <td rowspan="2">XSL Transformations</td>
        </tr>
        <tr>
          <td>2.00 p.m.</td>
          <td>5.00 p.m.</td>
        </tr>

        <tr>
          <td>Wednesday</td>
          <td>8:00 a.m.</td>
          <td>12:00 p.m.</td>
          <td>XSL Formatting Objects</td>
        </tr>
      </tbody>
    </table>
  </body>
</html>
```

---

### Clone a picture of form

![Contact Form Home Work](/01%20-%20HTML%20Basics/02%20-%20HTML%20Basics/contact%20form%20hw.png)

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <h1>Welcome to CodeHelp</h1>
    <h2>Contact Us Form</h2>
    <form action="">
      <div>
        <!-- Name  -->
        <label for="name">Name</label>
        <input type="text" name="name" id="" placeholder="Enter Your Name" />
      </div>

      <!-- Email  -->
      <div>
        <label for="email">Email</label>
        <input type="email" name="email" id="" placeholder="Enter Your Email" />
      </div>

      <!-- Contact Number  -->
      <div>
        <label for="contact-number">Contact Number</label>
        <input type="number" name="contact-number" id="" />
      </div>

      <!-- Gender  -->
      <div>
        <label for="gender">Gender</label>
        <select name="gender" id="">
          <option value="male">Male</option>
          <option value="female">Female</option>
        </select>
      </div>

      <!-- Date of Birth  -->
      <div>
        <label for="date-of-birth">Contact Number</label>
        <input type="date" name="date-of-birth" id="" />
      </div>

      <!-- Rating  -->
      <div>
        <label for="rating">Rating</label>
        <input type="radio" name="rating" id="" value="1" />1
        <input type="radio" name="rating" id="" value="2" />2
        <input type="radio" name="rating" id="" value="3" />3
        <input type="radio" name="rating" id="" value="4" />4
        <input type="radio" name="rating" id="" value="5" />5
      </div>

      <!-- Message  -->
      <div>
        <label for="message">Enter Your Message</label>
        <br />
        <textarea
          name="message"
          id=""
          cols="40"
          rows="5"
          placeholder="Enter Your Message"
        ></textarea>
      </div>
    </form>
  </body>
</html>
```

---
