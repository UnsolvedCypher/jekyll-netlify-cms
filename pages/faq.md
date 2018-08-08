---
title: Frequently asked questions
permalink: /faq
layout: default
extra_head: |
  <link href='https://fonts.googleapis.com/css?family=Open+Sans:400,300,600,700' rel='stylesheet' type='text/css'>

  <link rel="stylesheet" href="css/reset.css"> <!-- CSS reset -->
  <link rel="stylesheet" href="css/faq.css"> <!-- Resource style -->
  <script src="js/modernizr.js"></script> <!-- Modernizr -->
heading: Frequently Asked Questions
subheading: Your questions, answered
bg-class: bg-4
---

<!-- <header>
	<h1>FAQ Template</h1>
</header> -->
<section class="cd-faq">
	<ul class="cd-faq-categories">
    {% for faq_section in site.data.faq_sections %}
		<li>
      <a {% if faq_section.name == site.data.faq_sections[0].name %} class="selected" {% endif %} href="#{{ faq_section.name }}">{{ faq_section.name }}</a>
    </li>
    {% endfor %}
	</ul> <!-- cd-faq-categories -->

	<div class="cd-faq-items">

    {% for faq_section in site.data.faq_sections %}

		<ul id="{{ faq_section.name }}" class="cd-faq-group">
			<li class="cd-faq-title"><h2>{{ faq_section.name }}</h2></li>
      {% for faq in site.data.faqs %}
      {% if faq.section != faq_section.name %}
      {% continue %}
      {% endif %}
			<li>
				<a class="cd-faq-trigger" href="#0">{{ faq.question }}</a>
				<div class="cd-faq-content">
					<p>{{ faq.answer }}</p>
				</div> <!-- cd-faq-content -->
			</li>
      {% endfor %}
		</ul> <!-- cd-faq-group -->
    {% endfor %}
	</div> <!-- cd-faq-items -->
	<a href="#0" class="cd-close-panel">Close</a>
</section> <!-- cd-faq -->
<script src="js/jquery-2.1.1.js"></script>
<script src="js/jquery.mobile.custom.min.js"></script>
<script src="js/main.js"></script> <!-- Resource jQuery -->
