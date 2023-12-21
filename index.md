---
layout: page
title: About Me
image: assets/images/profile_pic2.jpg
nav-menu: true
order: 1
---

{% assign data = site.data.personal %}
<div id="main" class="alt">
	<!-- Two -->
	<section id="one">
		<div class="inner no-padding">
			<div>
				<p class='actions'>{{ data.description }}</p>
			</div>
			<div class="row">
				<div class="6u 12u$(small)">
					<div class="table-container">
					<table>
						{% for d in data.details %}
						<tr>
							<td class="first-column"><a href="#" class="special small disable">{{ d.key }}</a></td>
							<td class="second-column"><a href="#" class="small disable">{{ d.value }}</a></td>
						</tr>
						{% endfor %}
					</table>
					</div>
				</div>
				<div class="6u$ 12u$(small)">
					<!-- <h3>Technologies</h3> -->
					<div class='logos-container'>
					</div>
				</div>
			</div>
		</div>
	</section>
	<section id="one">
		<div class="inner no-padding">
			<div class="row">
				<div class="6u 12u$(small)">
					<header class="major">
						<h1>Fields of Interest</h1>
					</header>
					<p class='actions'> 
						{% for d in data.fields_of_interest %}
						<a href="#" class="button small disable">{{ d }}</a>
						{% endfor %}
					</p>
				</div>
				<div class="6u$ 12u$(small)">
					<header class="major">
						<h1>Soft Skills</h1>
					</header>
					<p class='actions'>
						{% for d in data.soft_skills %}
						<a href="#" class="button small disable">{{ d }}</a>
						{% endfor %}
					</p>
				</div>
				<div class="6u$ 12u$(small)">
					<header class="major">
						<h1>Technologies</h1>
					</header>
					<div class='logos-container'>
						<img src="{{site.baseurl}}/assets/images/logos/python.png" alt="python" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/java.png" alt="java" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/C++.png" alt="C++" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/php.png" alt="php" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/CSS.png" alt="CSS" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/JS.png" alt="JS" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/node.png" alt="node" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/html.png" alt="CSS" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/bash.png" alt="bash" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/git.png" alt="git" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/github_actions.png" alt="github_actions" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/PyPI.png" alt="pypi" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/numpy.png" alt="numpy" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/pandas.png" alt="pandas" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/sk_learn.png" alt="sk_learn" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/nltk.png" alt="nltk" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/beautifulsoup.png" alt="beautifulsoup" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/cv2.png" alt="cv2" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/keras.png" alt="keras" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/tensorflow.png" alt="tensorflow" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/PyTorch.png" alt="PyTorch" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/matplotlib.png" alt="matplotlib" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/seaborn.png" alt="seaborn" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/plotly.png" alt="plotly" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/django.png" alt="django" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/flask.png" alt="flask" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/fastapi.png" alt="fastapi" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/elasticsearch.png" alt="elasticsearch" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/travisCI.png" alt="travisCI" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/jenkins.png" alt="jenkins" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/mongodb.png" alt="mongodb" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/my_sql.png" alt="my_sql" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/postgre_sql.png" alt="postgre_sql" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/aws.png" alt="aws" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/cloud-logo.svg" alt="aws" class="logos">
						<img src="{{site.baseurl}}/assets/images/logos/docker.png" alt="docker" class="logos">
					</div>
				</div>
			</div>
		</div>
	</section>
	<section id='second'>
		<div class='inner no-padding'>
			<header class="major">
				<h1>Certificates</h1>
			</header>
			<ul class="fa-ul">
				{% for d in data.certificates %}
				<li>
					<i class="fa-li fa fa-check-square"></i>{{ d.title }}
					<a href="{{ d.link }}">
						<i class="fas fa-arrow-right"></i>
						{{ d.title }}
					</a>
				</li>
				{% endfor %}
			</ul>
		</div>
	</section>
</div>