# Dmitry (Gauthier) Chernigov

### Contact Info
  * **tel:** +7 (911) 795-79-99
  * **email:** dmitrygauthier@gmail.com
  * **telegram:** @gauthier

### Summary
  I’m a Web Developer with 8+ years of experience in both Web Development and freelance. I studied IT in university and graduated with a Specialist Degree (in different countries can be interpreted as an equivalent of a Bachelor’s or Master’s degree). I worked on the design and development of online stores, feedback forms, creation of support chats, landing page design, article editing for online publishers, randomizers, development of activity statistics data on social media, etc. I am an experienced professional, able to fulfill many tasks and do it well, familiar with all the ins and outs of my job.

### Skills
  * PHP, SQL Database (MySQL, PDO)
  * HTML5, CSS, JavaScript
  * Apache HTTP Server
  * Linux, Ubuntu
  * Object-oriented programming
  * Adobe Photoshop/Illustrator/Lightroom

### Code example
```JavaScript
const ajax = (method, options) => {
    let o = options || {},
		method = method,
		xhr;

	let url = o[0];
	let act = this.encurl(o[1]);

	let success = o[2];
			
	if (typeof o[3] === 'function') {
		let errors = o[3];
		let json = o[4] || false;
	} else {
		let json = o[3];
	}

	if (w.XMLHttpRequest) { // good browsers & ie7+
		xhr = new XMLHttpRequest();
	} else { // ie5 or ie6
		xhr = new ActiveXObject('Microsoft.XMLHTTP');
	}

	xhr.addEventListener('readystatechange', function() {
		if (this.readyState == 4 && this.status >= 200) {
			if (typeof success === 'function') {
				if (json === true) {
					success(JSON.parse(this.responseText));
				} else {
					success(this.responseText);
				}
			}

			if (typeof errors === 'function') {
				errors();
			}
		}
	});

	if (method == 'get') {
		xhr.open('GET', url, true);
		xhr.send();
	} else if(method == 'post') {
		xhr.open('POST', url);
		xhr.setRequestHeader('Content-Type','application/x-www-form-urlencoded;');
		xhr.send(act);
	} else if(method == 'upload') {
		xhr.open('POST', url);
		xhr.send(act);
	}
};
```

### Education
  * **2007 - 2012** - St.-Petersburg State Polytechnical University (Bachelor of Science in Information Technology, Engineering physics)

Courses:
  * **2010** - St.-Petersburg State Polytechnical University, Faculty of Specialists training (DEV-P10. Web-Programming usign PHP and MySQL)

### English
  A2 (Pre-Intermediate)
