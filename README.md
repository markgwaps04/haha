@import url(font-awesome.min.css);
@import url("https://fonts.googleapis.com/css?family=Source+Sans+Pro:300,400,300i,400i");



/* Reset */

	html, body, div, span, applet, object, iframe, h1, h2, h3, h4, h5, h6, p, blockquote, pre, a, abbr, acronym, address, big, cite, code, del, dfn, em, img, ins, kbd, q, s, samp, small, strike, strong, sub, sup, tt, var, b, u, i, center, dl, dt, dd, ol, ul, li, fieldset, form, label, legend, table, caption, tbody, tfoot, thead, tr, th, td, article, aside, canvas, details, embed, figure, figcaption, footer, header, hgroup, menu, nav, output, ruby, section, summary, time, mark, audio, video {
		margin: 0;
		padding: 0;
		border: 0;
		font-size: 100%;
		font: inherit;
		vertical-align: baseline;
	}

	article, aside, details, figcaption, figure, footer, header, hgroup, menu, nav, section {
		display: block;
	}

	body {
		line-height: 1;
	}

	ol, ul {
		list-style: none;
	}

	blockquote, q {
		quotes: none;
	}

	blockquote:before, blockquote:after, q:before, q:after {
		content: '';
		content: none;
	}

	table {
		border-collapse: collapse;
		border-spacing: 0;
	}

	body {
		-webkit-text-size-adjust: none;
	}

/* Box Model */

	*, *:before, *:after {
		-moz-box-sizing: border-box;
		-webkit-box-sizing: border-box;
		box-sizing: border-box;
	}

/* Page */

	@-moz-keyframes load-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@-webkit-keyframes load-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@-ms-keyframes load-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@keyframes load-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@-ms-viewport {
		width: device-width;
	}

	html {
		width: 100%;
		height: 100%;
	}

	body {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-align-items: center;
		-webkit-align-items: center;
		-ms-align-items: center;
		align-items: center;
		-moz-justify-content: -moz-flex-start;
		-webkit-justify-content: -webkit-flex-start;
		-ms-justify-content: -ms-flex-start;
		justify-content: flex-start;
		-ms-overflow-style: scrollbar;
		width: 100%;
		height: 100%;
		min-height: 30rem;
		overflow: hidden;
	}

		body:before {
			-moz-animation: load-spinner 1s infinite linear;
			-webkit-animation: load-spinner 1s infinite linear;
			-ms-animation: load-spinner 1s infinite linear;
			animation: load-spinner 1s infinite linear;
			-moz-transition: opacity 0.25s ease;
			-webkit-transition: opacity 0.25s ease;
			-ms-transition: opacity 0.25s ease;
			transition: opacity 0.25s ease;
			-moz-transition-delay: 0s;
			-webkit-transition-delay: 0s;
			-ms-transition-delay: 0s;
			transition-delay: 0s;
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
			content: '';
			display: block;
			position: absolute;
			top: 50%;
			left: 50%;
			width: 4rem;
			height: 4rem;
			margin: -2rem 0 0 -2rem;
			background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' width='96px' height='96px' viewBox='0 0 96 96' zoomAndPan='disable'%3E%3Cstyle%3Ecircle %7Bfill: transparent%3B stroke: %232e2b37%3B stroke-width: 1.5px%3B %7D%3C/style%3E%3Cdefs%3E%3CclipPath id='corner'%3E%3Cpolygon points='0,0 48,0 48,48 96,48 96,96 0,96' /%3E%3C/clipPath%3E%3C/defs%3E%3Cg clip-path='url(%23corner)'%3E%3Ccircle cx='48' cy='48' r='32'/%3E%3C/g%3E%3C/svg%3E");
			background-position: center;
			background-repeat: no-repeat;
			background-size: 4rem;
			opacity: 0;
		}

		body:after {
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
			content: '';
			display: block;
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			z-index: -1;
			background-attachment: fixed;
			background-color: #e1e6e1;
			background-image: url("../../images/overlay.png"), url("../../images/bg.jpg");
			background-repeat: repeat, repeat-x;
			background-size: 128px 128px, cover;
		}

		body.is-loading *, body.is-loading *:before, body.is-loading *:after {
			-moz-animation: none !important;
			-webkit-animation: none !important;
			-ms-animation: none !important;
			animation: none !important;
			-moz-transition: none !important;
			-webkit-transition: none !important;
			-ms-transition: none !important;
			transition: none !important;
		}

		body.is-loading:before {
			-moz-transition: opacity 1s ease;
			-webkit-transition: opacity 1s ease;
			-ms-transition: opacity 1s ease;
			transition: opacity 1s ease;
			-moz-transition-delay: 0.75s;
			-webkit-transition-delay: 0.75s;
			-ms-transition-delay: 0.75s;
			transition-delay: 0.75s;
			opacity: 0.25;
		}

	@media screen and (max-width: 736px) {

		html {
			height: auto;
		}

		body {
			height: auto;
			overflow-x: hidden;
			overflow-y: auto;
		}

	}

	@media screen and (max-width: 480px) {

		html, body {
			min-width: 320px;
		}

	}

/* Typography */

	html {
		font-size: 18pt;
		font-size: 1vmax;
	}

		@media screen and (max-width: 1680px) {

			html {
				font-size: 12pt;
				font-size: 1.1vmax;
			}

		}

		@media screen and (max-width: 1280px) {

			html {
				font-size: 11pt;
				font-size: 1.5vmax;
			}

		}

	body, input, select, textarea {
		color: rgba(255, 255, 255, 0.75);
		font-family: "Source Sans Pro", Helvetica, sans-serif;
		font-size: 1rem;
		font-weight: 300;
		line-height: 1.65;
	}

	a {
		-moz-transition: color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		-webkit-transition: color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		-ms-transition: color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		transition: color 0.2s ease-in-out, border-bottom-color 0.2s ease-in-out;
		color: inherit;
		border-bottom: dotted 1px;
		text-decoration: none;
	}

		a:hover {
			border-bottom-color: transparent;
			color: #ffe4b4;
		}

	strong, b {
		color: rgba(255, 255, 255, 0.875);
		font-weight: 400;
	}

	em, i {
		font-style: italic;
	}

	p {
		margin: 0 0 1.5rem 0;
	}

		body.is-ie p {
			width: 100%;
		}

	h1, h2, h3, h4, h5, h6 {
		color: rgba(255, 255, 255, 0.875);
		font-family: Arial, Helvetica, sans-serif;
		font-weight: 700;
		line-height: 1.3;
		margin: 0 0 0.75rem 0;
		letter-spacing: -0.05em;
	}

		h1 a, h2 a, h3 a, h4 a, h5 a, h6 a {
			color: inherit;
			text-decoration: none;
		}

	h1.major, h2.major, h3.major {
		position: relative;
	}

		h1.major:after, h2.major:after, h3.major:after {
			content: '';
			position: absolute;
			left: 0;
			width: 3.5rem;
			height: 0.1rem;
			background-color: rgba(255, 255, 255, 0.25);
		}

	h1 {
		font-size: 3rem;
		line-height: 1.2;
	}

		h1.major {
			margin: 0 0 2.625rem 0;
		}

			h1.major:after {
				bottom: -1.325rem;
			}

	h2 {
		font-size: 1.75rem;
		line-height: 1.2;
	}

		h2.major {
			margin: 0 0 1.9875rem 0;
		}

			h2.major:after {
				bottom: -1.2rem;
			}

	h3 {
		font-size: 1.325rem;
	}

		h3.major {
			margin: 0 0 1.875rem 0;
		}

			h3.major:after {
				bottom: -0.75rem;
			}

	h4 {
		font-size: 1rem;
	}

	h5 {
		font-size: 0.9rem;
	}

	h6 {
		font-size: 0.7rem;
	}

	sub {
		font-size: 0.8rem;
		position: relative;
		top: 0.5rem;
	}

	sup {
		font-size: 0.8rem;
		position: relative;
		top: -0.5rem;
	}

	blockquote {
		border-left: solid 0.25rem rgba(255, 255, 255, 0.25);
		font-style: italic;
		margin: 0 0 1.5rem 0;
		padding: 0.375rem 0 0.375rem 1.5rem;
	}

	code {
		background: rgba(255, 255, 255, 0.075);
		border-radius: 0.25rem;
		font-family: "Courier New", monospace;
		font-size: 0.8rem;
		margin: 0 0.25rem;
		padding: 0.25rem 0.65rem;
	}

	pre {
		-webkit-overflow-scrolling: touch;
		font-family: "Courier New", monospace;
		font-size: 0.8rem;
		margin: 0 0 1.5rem 0;
		white-space: pre-wrap;
	}

		pre code {
			display: block;
			line-height: 1.625;
			padding: 1rem 1.5rem;
			overflow-x: auto;
			margin: 0;
		}

	hr {
		border: 0;
		border-bottom: solid 2px rgba(255, 255, 255, 0.25);
		margin: 1.875rem 0;
	}

	.align-left {
		text-align: left;
	}

	.align-center {
		text-align: center;
	}

	.align-right {
		text-align: right;
	}

	@media screen and (max-width: 736px) {

		html {
			font-size: 12pt;
		}

		h1 {
			font-size: 2.25rem;
			line-height: 1.2;
		}

			h1.major {
				margin: 0 0 2.625rem 0;
			}

				h1.major:after {
					bottom: -1.325rem;
				}

		h2 {
			font-size: 1.5rem;
			line-height: 1.2;
		}

			h2.major {
				margin: 0 0 1.9875rem 0;
			}

				h2.major:after {
					bottom: -1.2rem;
				}

		h3 {
			font-size: 1rem;
		}

			h3.major {
				margin: 0 0 1.875rem 0;
			}

				h3.major:after {
					bottom: -0.75rem;
				}

		h4 {
			font-size: 1rem;
		}

		h5 {
			font-size: 0.9rem;
		}

		h6 {
			font-size: 0.7rem;
		}

		h1 br, h2 br, h3 br, h4 br, h5 br, h6 br {
			display: none;
		}

	}

	@media screen and (max-width: 360px) {

		html {
			font-size: 11pt;
		}

	}

/* Form */

	form {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-flex-wrap: wrap;
		-webkit-flex-wrap: wrap;
		-ms-flex-wrap: wrap;
		flex-wrap: wrap;
		width: calc(100% + 3rem);
		margin: -1.5rem 0 1.5rem -1.5rem;
	}

		form > .field {
			-moz-flex-grow: 0;
			-webkit-flex-grow: 0;
			-ms-flex-grow: 0;
			flex-grow: 0;
			-moz-flex-shrink: 0;
			-webkit-flex-shrink: 0;
			-ms-flex-shrink: 0;
			flex-shrink: 0;
			padding: 1.5rem 0 0 1.5rem;
			width: calc(100% - 1.5rem);
		}

			form > .field.half {
				width: calc(50% - 0.75rem);
			}

			form > .field.third {
				width: calc(100%/3 - 0.5rem);
			}

			form > .field.quarter {
				width: calc(25% - 0.375rem);
			}

		form > .actions {
			-moz-flex-grow: 0;
			-webkit-flex-grow: 0;
			-ms-flex-grow: 0;
			flex-grow: 0;
			-moz-flex-shrink: 1;
			-webkit-flex-shrink: 1;
			-ms-flex-shrink: 1;
			flex-shrink: 1;
			margin: 1.5rem 0 0 1.5rem;
		}

	label {
		color: rgba(255, 255, 255, 0.875);
		display: block;
		font-family: Arial, Helvetica, sans-serif;
		font-size: 0.8rem;
		font-weight: 700;
		margin: 0 0 0.4875rem 0;
	}

	input[type="text"],
	input[type="password"],
	input[type="email"],
	input[type="tel"],
	select,
	textarea {
		-moz-appearance: none;
		-webkit-appearance: none;
		-ms-appearance: none;
		appearance: none;
		background: transparent;
		border: solid 2px rgba(255, 255, 255, 0.25);
		border-radius: 0.25rem;
		color: inherit;
		display: block;
		outline: 0;
		padding: 0 0.75rem;
		text-decoration: none;
		width: 100%;
	}

		input[type="text"]:invalid,
		input[type="password"]:invalid,
		input[type="email"]:invalid,
		input[type="tel"]:invalid,
		select:invalid,
		textarea:invalid {
			box-shadow: none;
		}

		input[type="text"]:focus,
		input[type="password"]:focus,
		input[type="email"]:focus,
		input[type="tel"]:focus,
		select:focus,
		textarea:focus {
			border-color: #ffe4b4;
		}

	option {
		background-color: rgba(255, 255, 255, 0.875);
		color: #2e2b37;
	}

	.select-wrapper {
		text-decoration: none;
		display: block;
		position: relative;
	}

		.select-wrapper:before {
			-moz-osx-font-smoothing: grayscale;
			-webkit-font-smoothing: antialiased;
			font-family: FontAwesome;
			font-style: normal;
			font-weight: normal;
			text-transform: none !important;
		}

		.select-wrapper:before {
			display: block;
			content: '\f107';
			position: absolute;
			top: 0;
			right: 0;
			width: 2.5rem;
			height: 2.5rem;
			line-height: 2.5rem;
			color: rgba(255, 255, 255, 0.75);
			pointer-events: none;
			text-align: center;
		}

			body.is-ie .select-wrapper:before {
				line-height: 2.5;
			}

		.select-wrapper select::-ms-expand {
			display: none;
		}

	input[type="text"],
	input[type="password"],
	input[type="email"],
	select {
		height: 2.5rem;
	}

	textarea {
		padding: 0.75rem 1rem;
	}

	input[type="checkbox"],
	input[type="radio"] {
		-moz-appearance: none;
		-webkit-appearance: none;
		-ms-appearance: none;
		appearance: none;
		display: block;
		float: left;
		margin-right: -2rem;
		opacity: 0;
		width: 1rem;
		z-index: -1;
	}

		input[type="checkbox"] + label,
		input[type="radio"] + label {
			text-decoration: none;
			position: relative;
			color: rgba(255, 255, 255, 0.75);
			cursor: pointer;
			display: inline-block;
			font-size: 1rem;
			font-weight: 300;
			margin-bottom: 0;
			padding-left: 2.5rem;
			padding-right: 1rem;
		}

			input[type="checkbox"] + label:before,
			input[type="radio"] + label:before {
				-moz-osx-font-smoothing: grayscale;
				-webkit-font-smoothing: antialiased;
				font-family: FontAwesome;
				font-style: normal;
				font-weight: normal;
				text-transform: none !important;
			}

			input[type="checkbox"] + label:before,
			input[type="radio"] + label:before {
				content: '';
				display: inline-block;
				position: absolute;
				top: 0;
				left: 0;
				width: 1.5rem;
				height: 1.5rem;
				line-height: 1.4375rem;
				background: rgba(255, 255, 255, 0.075);
				border: solid 1px rgba(255, 255, 255, 0.25);
				border-radius: 0.25rem;
				color: #2e2b37;
				text-align: center;
			}

				body.is-ie input[type="checkbox"] + label:before, body.is-ie
				input[type="radio"] + label:before {
					line-height: 1.5;
				}

		input[type="checkbox"]:checked + label:before,
		input[type="radio"]:checked + label:before {
			content: '\f00c';
			background: rgba(255, 255, 255, 0.875);
			border-color: rgba(255, 255, 255, 0.875);
		}

		input[type="checkbox"]:focus + label:before,
		input[type="radio"]:focus + label:before {
			border-color: #ffe4b4;
			box-shadow: 0 0 0 1px #ffe4b4;
		}

		input[type="checkbox"]:focus:checked + label:before,
		input[type="radio"]:focus:checked + label:before {
			background: #ffe4b4;
		}

		input[type="checkbox"].color1 + label:before,
		input[type="radio"].color1 + label:before {
			color: #726193;
		}

		input[type="checkbox"].color2 + label:before,
		input[type="radio"].color2 + label:before {
			color: #e37b7c;
		}

		input[type="checkbox"].color3 + label:before,
		input[type="radio"].color3 + label:before {
			color: #ffe4b4;
		}

		input[type="checkbox"].color4 + label:before,
		input[type="radio"].color4 + label:before {
			color: #353865;
		}

	input[type="checkbox"] + label:before {
		border-radius: 0.25rem;
	}

	input[type="radio"] + label:before {
		border-radius: 100%;
	}

	::-webkit-input-placeholder {
		color: rgba(255, 255, 255, 0.5) !important;
		opacity: 1.0;
	}

	:-moz-placeholder {
		color: rgba(255, 255, 255, 0.5) !important;
		opacity: 1.0;
	}

	::-moz-placeholder {
		color: rgba(255, 255, 255, 0.5) !important;
		opacity: 1.0;
	}

	:-ms-input-placeholder {
		color: rgba(255, 255, 255, 0.5) !important;
		opacity: 1.0;
	}

	.formerize-placeholder {
		color: rgba(255, 255, 255, 0.5) !important;
		opacity: 1.0;
	}

	@media screen and (max-width: 736px) {

		form {
			margin: -1.5rem 0 1.5rem 0;
			width: 100%;
		}

			form > .field {
				padding: 1.5rem 0 0 0;
				width: 100% !important;
			}

			form > .actions {
				margin: 1.5rem 0 0 0;
			}

	}

/* Icon */

	.icon {
		text-decoration: none;
		position: relative;
		border-bottom: none;
	}

		.icon:before {
			-moz-osx-font-smoothing: grayscale;
			-webkit-font-smoothing: antialiased;
			font-family: FontAwesome;
			font-style: normal;
			font-weight: normal;
			text-transform: none !important;
		}

		.icon > .label {
			display: none;
		}

/* Image */

	.image {
		display: inline-block;
		position: relative;
		border: 0;
	}

		.image.filtered:after {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
			background-size: 128px 128px, auto;
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
			content: '';
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			opacity: 1;
			z-index: 1;
		}

		.image.filtered.tinted:after {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25)), linear-gradient(0deg, rgba(0, 0, 0, 0.125), rgba(0, 0, 0, 0.125));
			background-size: 128px 128px, auto, auto;
		}

		.image[data-position] img {
			-moz-object-fit: cover;
			-webkit-object-fit: cover;
			-ms-object-fit: cover;
			object-fit: cover;
			display: block;
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
		}

		.image[data-position="top left"] img {
			-moz-object-position: top left;
			-webkit-object-position: top left;
			-ms-object-position: top left;
			object-position: top left;
		}

		.image[data-position="top"] img {
			-moz-object-position: top;
			-webkit-object-position: top;
			-ms-object-position: top;
			object-position: top;
		}

		.image[data-position="top right"] img {
			-moz-object-position: top right;
			-webkit-object-position: top right;
			-ms-object-position: top right;
			object-position: top right;
		}

		.image[data-position="right"] img {
			-moz-object-position: right;
			-webkit-object-position: right;
			-ms-object-position: right;
			object-position: right;
		}

		.image[data-position="bottom right"] img {
			-moz-object-position: bottom right;
			-webkit-object-position: bottom right;
			-ms-object-position: bottom right;
			object-position: bottom right;
		}

		.image[data-position="bottom"] img {
			-moz-object-position: bottom;
			-webkit-object-position: bottom;
			-ms-object-position: bottom;
			object-position: bottom;
		}

		.image[data-position="bottom left"] img {
			-moz-object-position: bottom left;
			-webkit-object-position: bottom left;
			-ms-object-position: bottom left;
			object-position: bottom left;
		}

		.image[data-position="left"] img {
			-moz-object-position: left;
			-webkit-object-position: left;
			-ms-object-position: left;
			object-position: left;
		}

		.image[data-position="center"] img {
			-moz-object-position: center;
			-webkit-object-position: center;
			-ms-object-position: center;
			object-position: center;
		}

		.image[data-position="25% 25%"] img {
			-moz-object-position: 25% 25%;
			-webkit-object-position: 25% 25%;
			-ms-object-position: 25% 25%;
			object-position: 25% 25%;
		}

		.image[data-position="75% 25%"] img {
			-moz-object-position: 75% 25%;
			-webkit-object-position: 75% 25%;
			-ms-object-position: 75% 25%;
			object-position: 75% 25%;
		}

		.image[data-position="75% 75%"] img {
			-moz-object-position: 75% 75%;
			-webkit-object-position: 75% 75%;
			-ms-object-position: 75% 75%;
			object-position: 75% 75%;
		}

		.image[data-position="25% 75%"] img {
			-moz-object-position: 25% 75%;
			-webkit-object-position: 25% 75%;
			-ms-object-position: 25% 75%;
			object-position: 25% 75%;
		}

		.image img {
			display: block;
		}

		.image.left, .image.right {
			max-width: 40%;
		}

			.image.left img, .image.right img {
				width: 100%;
			}

		.image.left {
			float: left;
			padding: 0 1.5rem 1rem 0;
			top: 0.25rem;
		}

		.image.right {
			float: right;
			padding: 0 0 1rem 1.5rem;
			top: 0.25rem;
		}

		.image.fit {
			display: block;
			margin: 0 0 1.5rem 0;
			width: 100%;
		}

			.image.fit img {
				width: 100%;
			}

		.image.main {
			display: block;
			margin: 0 0 2.25rem 0;
			width: 100%;
		}

			.image.main img {
				width: 100%;
			}

/* List */

	ol {
		list-style: decimal;
		margin: 0 0 1.5rem 0;
		padding-left: 1.25rem;
	}

		ol li {
			padding-left: 0.25rem;
		}

	ul {
		list-style: disc;
		margin: 0 0 1.5rem 0;
		padding-left: 1rem;
	}

		ul li {
			padding-left: 0.5rem;
		}

		ul.alt {
			list-style: none;
			padding-left: 0;
		}

			ul.alt li {
				border-top: solid 1px rgba(255, 255, 255, 0.25);
				padding: 0.5rem 0;
			}

				ul.alt li:first-child {
					border-top: 0;
					padding-top: 0;
				}

		ul.icons {
			cursor: default;
			list-style: none;
			padding-left: 0;
		}

			ul.icons li {
				display: inline-block;
				padding: 0 1rem 0 0;
			}

				ul.icons li:last-child {
					padding-right: 0;
				}

				ul.icons li .icon:before {
					font-size: 1.25em;
				}

		ul.actions {
			cursor: default;
			list-style: none;
			padding-left: 0;
		}

			ul.actions li {
				display: inline-block;
				padding: 0 0.75rem 0 0;
				vertical-align: middle;
			}

				ul.actions li:last-child {
					padding-right: 0;
				}

			ul.actions.small li {
				padding: 0 0.375rem 0 0;
			}

			ul.actions.vertical li {
				display: block;
				padding: 0.75rem 0 0 0;
			}

				ul.actions.vertical li:first-child {
					padding-top: 0;
				}

				ul.actions.vertical li > * {
					margin-bottom: 0;
				}

			ul.actions.vertical.small li {
				padding: 0.375rem 0 0 0;
			}

				ul.actions.vertical.small li:first-child {
					padding-top: 0;
				}

			ul.actions.fit {
				display: table;
				margin-left: -0.75rem;
				padding: 0;
				table-layout: fixed;
				width: calc(100% + 0.75rem);
			}

				ul.actions.fit li {
					display: table-cell;
					padding: 0 0 0 0.75rem;
				}

					ul.actions.fit li > * {
						margin-bottom: 0;
					}

				ul.actions.fit.small {
					margin-left: -0.375rem;
					width: calc(100% + 0.375rem);
				}

					ul.actions.fit.small li {
						padding: 0 0 0 0.375rem;
					}

		ul.contact-icons {
			list-style: none;
			padding-left: 0;
		}

			ul.contact-icons > li {
				margin: 1.25rem 0 0 0;
				padding-left: 0;
			}

				ul.contact-icons > li:before {
					display: inline-block;
					width: 2.25rem;
					height: 2.25rem;
					line-height: 2.25rem;
					border-radius: 2.25rem;
					background-color: white;
					color: #2e2b37;
					cursor: default;
					font-size: 1.125rem;
					margin-right: 1rem;
					text-align: center;
					vertical-align: middle;
				}

					body.is-ie ul.contact-icons > li:before {
						line-height: 2.125;
					}

				ul.contact-icons > li a {
					border-bottom: 0;
				}

			ul.contact-icons.color1 > li:before {
				color: #726193;
			}

			ul.contact-icons.color2 > li:before {
				color: #e37b7c;
			}

			ul.contact-icons.color3 > li:before {
				color: #ffe4b4;
			}

			ul.contact-icons.color4 > li:before {
				color: #353865;
			}

		ul.grid-icons {
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-wrap: wrap;
			-webkit-flex-wrap: wrap;
			-ms-flex-wrap: wrap;
			flex-wrap: wrap;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			list-style: none;
			margin: 0 0 1.5rem 0;
			padding-left: 0;
		}

			ul.grid-icons .icon {
				display: block;
				position: relative;
				width: 100%;
				text-align: center;
			}

				ul.grid-icons .icon:before {
					display: block;
					width: 6rem;
					height: 6rem;
					line-height: 6rem;
					border-radius: 6rem;
					box-shadow: inset 0 0 0 2px rgba(255, 255, 255, 0.25);
					font-size: 2.5rem;
					margin: 0 auto;
					text-align: center;
				}

					body.is-ie ul.grid-icons .icon:before {
						line-height: 2.375;
					}

			ul.grid-icons > li {
				-moz-flex-grow: 0;
				-webkit-flex-grow: 0;
				-ms-flex-grow: 0;
				flex-grow: 0;
				-moz-flex-shrink: 0;
				-webkit-flex-shrink: 0;
				-ms-flex-shrink: 0;
				flex-shrink: 0;
				position: relative;
				margin: 1.5rem 0 0 1.5rem;
				padding-left: 0;
			}

			ul.grid-icons.connected > li:before {
				content: '';
				display: block;
				position: absolute;
				width: 1.5rem;
				height: 2px;
				top: 50%;
				left: -1.5rem;
				background-color: rgba(255, 255, 255, 0.25);
			}

			ul.grid-icons.connected > li:after {
				content: '';
				display: block;
				position: absolute;
				width: 2px;
				height: 1.5rem;
				top: -1.5rem;
				left: 50%;
				background-color: rgba(255, 255, 255, 0.25);
			}

			ul.grid-icons.two {
				width: 14rem;
			}

				ul.grid-icons.two > li:nth-child(-n + 2) {
					margin-top: 0;
				}

					ul.grid-icons.two > li:nth-child(-n + 2):after {
						display: none;
					}

				ul.grid-icons.two > li:nth-child(2n - 1) {
					margin-left: 0;
				}

					ul.grid-icons.two > li:nth-child(2n - 1):before {
						display: none;
					}

			ul.grid-icons.three {
				width: 21.5rem;
			}

				ul.grid-icons.three > li:nth-child(-n + 3) {
					margin-top: 0;
				}

					ul.grid-icons.three > li:nth-child(-n + 3):after {
						display: none;
					}

				ul.grid-icons.three > li:nth-child(3n - 2) {
					margin-left: 0;
				}

					ul.grid-icons.three > li:nth-child(3n - 2):before {
						display: none;
					}

			ul.grid-icons.four {
				width: 29rem;
			}

				ul.grid-icons.four > li:nth-child(-n + 4) {
					margin-top: 0;
				}

					ul.grid-icons.four > li:nth-child(-n + 4):after {
						display: none;
					}

				ul.grid-icons.four > li:nth-child(4n - 3) {
					margin-left: 0;
				}

					ul.grid-icons.four > li:nth-child(4n - 3):before {
						display: none;
					}

	dl {
		margin: 0 0 1.5rem 0;
	}

		dl dt {
			display: block;
			font-weight: 400;
			margin: 0 0 0.75rem 0;
		}

		dl dd {
			margin-left: 1.5rem;
		}

	@media screen and (max-width: 736px) {

		ul.grid-icons {
			-moz-justify-content: -moz-flex-start;
			-webkit-justify-content: -webkit-flex-start;
			-ms-justify-content: -ms-flex-start;
			justify-content: flex-start;
			width: 100% !important;
			margin: -1rem 0 1.5rem -1rem;
		}

			ul.grid-icons .icon:before {
				width: 4.5rem;
				height: 4.5rem;
				line-height: 4.5rem;
				font-size: 1.75rem;
			}

			ul.grid-icons > li {
				margin: 1rem 0 0 1rem !important;
			}

				ul.grid-icons > li:before {
					display: none !important;
				}

				ul.grid-icons > li:after {
					display: none !important;
				}

	}

/* Table */

	.table-wrapper {
		-webkit-overflow-scrolling: touch;
		overflow-x: auto;
	}

	table {
		margin: 0 0 1.5rem 0;
		width: 100%;
	}

		table tbody tr {
			border: solid 1px rgba(255, 255, 255, 0.25);
			border-left: 0;
			border-right: 0;
		}

			table tbody tr:nth-child(2n + 1) {
				background-color: rgba(255, 255, 255, 0.075);
			}

		table td {
			padding: 0.75rem 0.75rem;
		}

		table th {
			color: rgba(255, 255, 255, 0.875);
			font-size: 0.9rem;
			font-weight: 400;
			padding: 0 0.75rem 0.75rem 0.75rem;
			text-align: left;
		}

		table thead {
			border-bottom: solid 2px rgba(255, 255, 255, 0.25);
		}

		table tfoot {
			border-top: solid 2px rgba(255, 255, 255, 0.25);
		}

		table.alt {
			border-collapse: separate;
		}

			table.alt tbody tr td {
				border: solid 1px rgba(255, 255, 255, 0.25);
				border-left-width: 0;
				border-top-width: 0;
			}

				table.alt tbody tr td:first-child {
					border-left-width: 1px;
				}

			table.alt tbody tr:first-child td {
				border-top-width: 1px;
			}

			table.alt thead {
				border-bottom: 0;
			}

			table.alt tfoot {
				border-top: 0;
			}

/* Button */

	input[type="submit"],
	input[type="reset"],
	input[type="button"]:not(.swal2-styled),
	button:not(.swal2-styled),
	.button:not(.swal2-styled) {
		-moz-appearance: none;
		-webkit-appearance: none;
		-ms-appearance: none;
		appearance: none;
		-moz-transition: background-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out, color 0.2s ease-in-out;
		-webkit-transition: background-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out, color 0.2s ease-in-out;
		-ms-transition: background-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out, color 0.2s ease-in-out;
		transition: background-color 0.2s ease-in-out, box-shadow 0.2s ease-in-out, color 0.2s ease-in-out;
		background-color: transparent;
		border: 0;
		border-radius: 0.25rem;
		box-shadow: inset 0 0 0 2px rgba(255, 255, 255, 0.25);
		color: rgba(255, 255, 255, 0.875) !important;
		cursor: pointer;
		display: inline-block;
		font-family: Arial, Helvetica, sans-serif;
		font-size: 0.6rem;
		font-weight: 700;
		height: 2.75rem;
		letter-spacing: 0.15rem;
		line-height: 2.75rem;
		padding: 0 1.5rem 0 1.65rem;
		text-align: center;
		text-decoration: none;
		text-transform: uppercase;
		white-space: nowrap;
	}

		input[type="submit"]:hover,
		input[type="reset"]:hover,
		input[type="button"]:not(.swal2-styled):hover,
		button:hover,
		.button:hover {
			box-shadow: inset 0 0 0 2px #ffe4b4;
			color: #ffe4b4 !important;
		}

		input[type="submit"]:active,
		input[type="reset"]:active,
		input[type="button"]:not(.swal2-styled):active,
		button:not(.swal2-styled):active,
		.button:not(.swal2-styled):active {
			background-color: rgba(255, 228, 180, 0.125);
		}

		input[type="submit"].icon:before,
		input[type="reset"].icon:before,
		input[type="button"].icon:before,
		button.icon:before,
		.button.icon:before {
			display: inline-block;
			position: relative;
			top: -0.075rem;
			vertical-align: middle;
			font-size: 0.8rem;
			margin: 0 0.375rem 0 -0.325rem;
		}

		input[type="submit"].icon.circle,
		input[type="reset"].icon.circle,
		input[type="button"].icon.circle,
		button.icon.circle,
		.button.icon.circle {
			position: relative;
			width: 3.125rem;
			height: 3.125rem;
			line-height: 3.125rem;
			text-indent: 3.125rem;
			border-radius: 100%;
			overflow: hidden;
			padding: 0;
			letter-spacing: 0;
		}

			input[type="submit"].icon.circle:before,
			input[type="reset"].icon.circle:before,
			input[type="button"].icon.circle:before,
			button.icon.circle:before,
			.button.icon.circle:before {
				display: block;
				position: absolute;
				top: 0;
				left: 0;
				width: inherit;
				height: inherit;
				font-size: 1.25rem;
				line-height: inherit;
				margin: 0;
				text-indent: 0;
			}

			input[type="submit"].icon.circle.fa-angle-left:before,
			input[type="reset"].icon.circle.fa-angle-left:before,
			input[type="button"].icon.circle.fa-angle-left:before,
			button.icon.circle.fa-angle-left:before,
			.button.icon.circle.fa-angle-left:before {
				position: relative;
				left: -0.1rem;
				font-size: 1.75rem;
			}

			input[type="submit"].icon.circle.fa-angle-right:before,
			input[type="reset"].icon.circle.fa-angle-right:before,
			input[type="button"].icon.circle.fa-angle-right:before,
			button.icon.circle.fa-angle-right:before,
			.button.icon.circle.fa-angle-right:before {
				position: relative;
				left: 0.1rem;
				font-size: 1.75rem;
			}

		input[type="submit"].fit,
		input[type="reset"].fit,
		input[type="button"].fit,
		button.fit,
		.button.fit {
			display: block;
			margin: 0 0 0.75rem 0;
			width: 100%;
		}

		input[type="submit"].small,
		input[type="reset"].small,
		input[type="button"].small,
		button.small,
		.button.small {
			font-size: 0.4rem;
			height: 1.875rem;
			line-height: 1.875rem;
			padding: 0 1.25rem 0 1.4rem;
		}

		input[type="submit"].large,
		input[type="reset"].large,
		input[type="button"].large,
		button.large,
		.button.large {
			font-size: 0.8rem;
			height: 3.3125rem;
			line-height: 3.3125rem;
			padding: 0 2rem 0 2.15rem;
		}

		input[type="submit"].special,
		input[type="reset"].special,
		input[type="button"].special,
		button.special,
		.button.special {
			background-color: white;
			box-shadow: none;
			color: #2e2b37 !important;
		}

			input[type="submit"].special.color1,
			input[type="reset"].special.color1,
			input[type="button"].special.color1,
			button.special.color1,
			.button.special.color1 {
				color: #726193 !important;
			}

			input[type="submit"].special.color2,
			input[type="reset"].special.color2,
			input[type="button"].special.color2,
			button.special.color2,
			.button.special.color2 {
				color: #e37b7c !important;
			}

			input[type="submit"].special.color3,
			input[type="reset"].special.color3,
			input[type="button"].special.color3,
			button.special.color3,
			.button.special.color3 {
				color: #ffe4b4 !important;
			}

			input[type="submit"].special.color4,
			input[type="reset"].special.color4,
			input[type="button"].special.color4,
			button.special.color4,
			.button.special.color4 {
				color: #353865 !important;
			}

			input[type="submit"].special:hover,
			input[type="reset"].special:hover,
			input[type="button"].special:hover,
			button.special:hover,
			.button.special:hover {
				background-color: #ffe4b4;
			}

			input[type="submit"].special:active,
			input[type="reset"].special:active,
			input[type="button"].special:active,
			button.special:active,
			.button.special:active {
				background-color: #fdd997;
			}

		input[type="submit"].disabled, input[type="submit"]:disabled,
		input[type="reset"].disabled,
		input[type="reset"]:disabled,
		input[type="button"].disabled:not(.swal2-styled),
		input[type="button"]:not(.swal2-styled):disabled,
		button.disabled:not(.swal2-styled),
		button:disabled:not(.swal2-styled),
		.button.disabled:not(.swal2-styled),
		.button:disabled:not(.swal2-styled) {
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
			cursor: default;
			opacity: 0.5;
		}

/* Gallery */

	@-moz-keyframes gallery-modal-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@-webkit-keyframes gallery-modal-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@-ms-keyframes gallery-modal-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	@keyframes gallery-modal-spinner {
		0% {
			-moz-transform: rotate(0deg);
			-webkit-transform: rotate(0deg);
			-ms-transform: rotate(0deg);
			transform: rotate(0deg);
		}

		100% {
			-moz-transform: rotate(360deg);
			-webkit-transform: rotate(360deg);
			-ms-transform: rotate(360deg);
			transform: rotate(360deg);
		}
	}

	.gallery {
		-moz-align-items: stretch;
		-webkit-align-items: stretch;
		-ms-align-items: stretch;
		align-items: stretch;
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		height: 100%;
	}

		.gallery > * {
			width: 20rem;
			height: 100%;
		}

		.gallery .image {
			display: block;
			position: relative;
			border-bottom: 0;
			overflow: hidden;
		}

			.gallery .image img {
				-moz-transition: -moz-transform 0.2s ease-in-out;
				-webkit-transition: -webkit-transform 0.2s ease-in-out;
				-ms-transition: -ms-transform 0.2s ease-in-out;
				transition: transform 0.2s ease-in-out;
			}

			.gallery .image:after {
				-moz-transition: opacity 0.2s ease-in-out;
				-webkit-transition: opacity 0.2s ease-in-out;
				-ms-transition: opacity 0.2s ease-in-out;
				transition: opacity 0.2s ease-in-out;
			}

			.gallery .image:hover img {
				-moz-transform: scale(1.025);
				-webkit-transform: scale(1.025);
				-ms-transform: scale(1.025);
				transform: scale(1.025);
			}

			.gallery .image:hover:after {
				opacity: 0;
			}

		.gallery .group {
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-wrap: wrap;
			-webkit-flex-wrap: wrap;
			-ms-flex-wrap: wrap;
			flex-wrap: wrap;
		}

			.gallery .group > * {
				height: 50%;
			}

		.gallery .modal {
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-align-items: center;
			-webkit-align-items: center;
			-ms-align-items: center;
			align-items: center;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
			-moz-user-select: none;
			-webkit-user-select: none;
			-ms-user-select: none;
			user-select: none;
			-moz-transition: opacity 0.5s ease, visibility 0.5s, z-index 0.5s;
			-webkit-transition: opacity 0.5s ease, visibility 0.5s, z-index 0.5s;
			-ms-transition: opacity 0.5s ease, visibility 0.5s, z-index 0.5s;
			transition: opacity 0.5s ease, visibility 0.5s, z-index 0.5s;
			-webkit-tap-highlight-color: transparent;
			position: fixed;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			background-color: rgba(46, 43, 55, 0.875);
			opacity: 0;
			outline: 0;
			visibility: none;
			z-index: 0;
		}

			.gallery .modal:before {
				-moz-animation: gallery-modal-spinner 1s infinite linear;
				-webkit-animation: gallery-modal-spinner 1s infinite linear;
				-ms-animation: gallery-modal-spinner 1s infinite linear;
				animation: gallery-modal-spinner 1s infinite linear;
				-moz-transition: opacity 0.25s ease;
				-webkit-transition: opacity 0.25s ease;
				-ms-transition: opacity 0.25s ease;
				transition: opacity 0.25s ease;
				-moz-transition-delay: 0.5s;
				-webkit-transition-delay: 0.5s;
				-ms-transition-delay: 0.5s;
				transition-delay: 0.5s;
				content: '';
				display: block;
				position: absolute;
				top: 50%;
				left: 50%;
				width: 4rem;
				height: 4rem;
				margin: -2rem 0 0 -2rem;
				background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' width='96px' height='96px' viewBox='0 0 96 96' zoomAndPan='disable'%3E%3Cstyle%3Ecircle %7Bfill: transparent%3B stroke: rgba(255, 255, 255, 0.875)%3B stroke-width: 1.5px%3B %7D%3C/style%3E%3Cdefs%3E%3CclipPath id='corner'%3E%3Cpolygon points='0,0 48,0 48,48 96,48 96,96 0,96' /%3E%3C/clipPath%3E%3C/defs%3E%3Cg clip-path='url(%23corner)'%3E%3Ccircle cx='48' cy='48' r='32'/%3E%3C/g%3E%3C/svg%3E");
				background-position: center;
				background-repeat: no-repeat;
				background-size: 4rem;
				opacity: 0;
			}

			.gallery .modal:after {
				content: '';
				display: block;
				position: absolute;
				top: 0.5rem;
				right: 0.5rem;
				width: 4rem;
				height: 4rem;
				background-image: url("data:image/svg+xml;charset=utf8,%3Csvg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' width='64px' height='64px' viewBox='0 0 64 64' zoomAndPan='disable'%3E%3Cstyle%3Eline %7Bstroke: rgba(255, 255, 255, 0.875)%3Bstroke-width: 1.5px%3B%7D%3C/style%3E%3Cline x1='20' y1='20' x2='44' y2='44' /%3E%3Cline x1='20' y1='44' x2='44' y2='20' /%3E%3C/svg%3E");
				background-position: center;
				background-repeat: no-repeat;
				background-size: 3rem;
				cursor: pointer;
			}

			.gallery .modal .inner {
				-moz-transform: translateY(0.75rem);
				-webkit-transform: translateY(0.75rem);
				-ms-transform: translateY(0.75rem);
				transform: translateY(0.75rem);
				-moz-transition: opacity 0.25s ease, -moz-transform 0.25s ease;
				-webkit-transition: opacity 0.25s ease, -webkit-transform 0.25s ease;
				-ms-transition: opacity 0.25s ease, -ms-transform 0.25s ease;
				transition: opacity 0.25s ease, transform 0.25s ease;
				opacity: 0;
			}

				.gallery .modal .inner img {
					display: block;
					max-width: 90vw;
					max-height: 85vh;
					box-shadow: 0 1rem 3rem 0 rgba(0, 0, 0, 0.35);
				}

			.gallery .modal.visible {
				-moz-pointer-events: auto;
				-webkit-pointer-events: auto;
				-ms-pointer-events: auto;
				pointer-events: auto;
				opacity: 1;
				visibility: visible;
				z-index: 11000;
			}

				.gallery .modal.visible:before {
					opacity: 1;
				}

			.gallery .modal.loaded .inner {
				-moz-transform: translateY(0);
				-webkit-transform: translateY(0);
				-ms-transform: translateY(0);
				transform: translateY(0);
				-moz-transition: opacity 0.5s ease, -moz-transform 0.5s ease;
				-webkit-transition: opacity 0.5s ease, -webkit-transform 0.5s ease;
				-ms-transition: opacity 0.5s ease, -ms-transform 0.5s ease;
				transition: opacity 0.5s ease, transform 0.5s ease;
				opacity: 1;
			}

			.gallery .modal.loaded:before {
				-moz-transition-delay: 0s;
				-webkit-transition-delay: 0s;
				-ms-transition-delay: 0s;
				transition-delay: 0s;
				opacity: 0;
			}

	@media screen and (max-width: 980px) {

		.gallery .modal .inner img {
			max-width: 100vw;
		}

	}

	@media screen and (max-width: 736px) {

		.gallery {
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			height: auto;
		}

			.gallery > * {
				height: auto;
				width: 100%;
			}

			.gallery .image {
				width: 100%;
				height: 40rem;
			}

			.gallery .group .span-0-25 {
				width: 8.33333%;
			}

			.gallery .group .span-0-5 {
				width: 16.66666%;
			}

			.gallery .group .span-0-75 {
				width: 25%;
			}

			.gallery .group .span-1 {
				width: 33.33333%;
			}

			.gallery .group .span-1-25 {
				width: 41.66666%;
			}

			.gallery .group .span-1-5 {
				width: 50%;
			}

			.gallery .group .span-1-75 {
				width: 58.33333%;
			}

			.gallery .group .span-2 {
				width: 66.66666%;
			}

			.gallery .group .span-2-25 {
				width: 74.99999%;
			}

			.gallery .group .span-2-5 {
				width: 83.33332%;
			}

			.gallery .group .span-2-75 {
				width: 91.66666%;
			}

			.gallery .group .span-3 {
				width: 99.99999%;
			}

			.gallery .group .span-3-25 {
				width: 108.33332%;
			}

			.gallery .group .span-3-5 {
				width: 116.66666%;
			}

			.gallery .group .span-3-75 {
				width: 124.99999%;
			}

			.gallery .group .span-4 {
				width: 133.33332%;
			}

			.gallery .group .span-4-25 {
				width: 141.66665%;
			}

			.gallery .group .span-4-5 {
				width: 149.99998%;
			}

			.gallery .group .span-4-75 {
				width: 158.33332%;
			}

			.gallery .group .span-5 {
				width: 166.66665%;
			}

			.gallery .group .span-5-25 {
				width: 174.99998%;
			}

			.gallery .group .span-5-5 {
				width: 183.33331%;
			}

			.gallery .group .span-5-75 {
				width: 191.66665%;
			}

			.gallery .group .span-6 {
				width: 199.99998%;
			}

			.gallery .group .span-6-25 {
				width: 208.33331%;
			}

			.gallery .group .span-6-5 {
				width: 216.66665%;
			}

			.gallery .group .span-6-75 {
				width: 224.99998%;
			}

			.gallery .group .span-7 {
				width: 233.33331%;
			}

			.gallery .group .span-7-25 {
				width: 241.66664%;
			}

			.gallery .group .span-7-5 {
				width: 249.99997%;
			}

			.gallery .group .span-7-75 {
				width: 258.33331%;
			}

			.gallery .group .span-8 {
				width: 266.66664%;
			}

			.gallery .group .span-8-25 {
				width: 274.99997%;
			}

			.gallery .group .span-8-5 {
				width: 283.33331%;
			}

			.gallery .group .span-8-75 {
				width: 291.66664%;
			}

			.gallery .group .span-9 {
				width: 299.99997%;
			}

			.gallery .group .span-9-25 {
				width: 308.3333%;
			}

			.gallery .group .span-9-5 {
				width: 316.66664%;
			}

			.gallery .group .span-9-75 {
				width: 324.99997%;
			}

			.gallery .group .span-10 {
				width: 333.3333%;
			}

			.gallery .group .image {
				height: 20rem;
			}

	}

	@media screen and (max-width: 480px) {

		.gallery .image {
			height: 30rem;
		}

		.gallery .group .image {
			height: 12.5rem;
		}

	}

/* Panel */

	.panel {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-flex-grow: 0;
		-webkit-flex-grow: 0;
		-ms-flex-grow: 0;
		flex-grow: 0;
		-moz-flex-shrink: 0;
		-webkit-flex-shrink: 0;
		-ms-flex-shrink: 0;
		flex-shrink: 0;
		-moz-justify-content: center;
		-webkit-justify-content: center;
		-ms-justify-content: center;
		justify-content: center;
		-moz-align-items: stretch;
		-webkit-align-items: stretch;
		-ms-align-items: stretch;
		align-items: stretch;
		height: 100%;
		overflow-x: hidden;
		overflow-y: auto;
	}

		.panel > * {
			position: relative;
			min-width: 10rem;
		}

			.panel > *.color0 {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, #726193 20%, #e37b7c 60%, #ffe4b4);
				background-size: 128px 128px, auto;
			}

			.panel > *.color1 {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #726193;
			}

			.panel > *.color2 {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #e37b7c;
			}

			.panel > *.color3 {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #ffe4b4;
			}

			.panel > *.color4 {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #353865;
			}

			.panel > *.color1-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #6c5e86;
			}

			.panel > *.color2-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #de7172;
			}

			.panel > *.color3-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #fedea6;
			}

			.panel > *.color4-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #323459;
			}

		.panel > .intro {
			padding: 3.5rem 3.5rem 2rem 3.5rem ;
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-grow: 0;
			-webkit-flex-grow: 0;
			-ms-flex-grow: 0;
			flex-grow: 0;
			-moz-flex-shrink: 0;
			-webkit-flex-shrink: 0;
			-ms-flex-shrink: 0;
			flex-shrink: 0;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			-moz-align-items: -moz-flex-start;
			-webkit-align-items: -webkit-flex-start;
			-ms-align-items: -ms-flex-start;
			align-items: flex-start;
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			width: 22rem;
		}

			.panel > .intro.joined {
				width: 18.5rem;
				padding-right: 0;
			}

				.panel > .intro.joined + .inner {
					padding-left: 2.625rem;
				}

		.panel > .inner {
			padding: 3.5rem 3.5rem 2rem 3.5rem ;
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-grow: 1;
			-webkit-flex-grow: 1;
			-ms-flex-grow: 1;
			flex-grow: 1;
			-moz-flex-shrink: 1;
			-webkit-flex-shrink: 1;
			-ms-flex-shrink: 1;
			flex-shrink: 1;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			-moz-align-items: -moz-flex-start;
			-webkit-align-items: -webkit-flex-start;
			-ms-align-items: -ms-flex-start;
			align-items: flex-start;
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			position: relative;
			width: 100%;
		}

			.panel > .inner.columns {
				display: -moz-flex;
				display: -webkit-flex;
				display: -ms-flex;
				display: flex;
				-moz-justify-content: center;
				-webkit-justify-content: center;
				-ms-justify-content: center;
				justify-content: center;
				-moz-align-items: center;
				-webkit-align-items: center;
				-ms-align-items: center;
				align-items: center;
				-moz-flex-direction: row;
				-webkit-flex-direction: row;
				-ms-flex-direction: row;
				flex-direction: row;
			}

				.panel > .inner.columns > * {
					-moz-flex-grow: 0;
					-webkit-flex-grow: 0;
					-ms-flex-grow: 0;
					flex-grow: 0;
					-moz-flex-shrink: 0;
					-webkit-flex-shrink: 0;
					-ms-flex-shrink: 0;
					flex-shrink: 0;
					margin-left: 3.5rem;
				}

				.panel > .inner.columns > :first-child {
					margin-left: 0;
				}

				.panel > .inner.columns.divided > * {
					margin-left: 7rem;
				}

					.panel > .inner.columns.divided > *:before {
						content: '';
						position: absolute;
						top: 3.5rem;
						width: 2px;
						height: calc(100% - 7rem);
						margin-left: -3.5rem;
						background-color: rgba(255, 255, 255, 0.25);
					}

				.panel > .inner.columns.divided > :first-child {
					margin-left: 0;
				}

					.panel > .inner.columns.divided > :first-child:before {
						display: none;
					}

				.panel > .inner.columns.aligned {
					-moz-align-items: -moz-flex-start;
					-webkit-align-items: -webkit-flex-start;
					-ms-align-items: -ms-flex-start;
					align-items: flex-start;
				}

		.panel .span-0-25 {
			width: 2.5rem;
		}

		.panel .span-0-5 {
			width: 5rem;
		}

		.panel .span-0-75 {
			width: 7.5rem;
		}

		.panel .span-1 {
			width: 10rem;
		}

		.panel .span-1-25 {
			width: 12.5rem;
		}

		.panel .span-1-5 {
			width: 15rem;
		}

		.panel .span-1-75 {
			width: 17.5rem;
		}

		.panel .span-2 {
			width: 20rem;
		}

		.panel .span-2-25 {
			width: 22.5rem;
		}

		.panel .span-2-5 {
			width: 25rem;
		}

		.panel .span-2-75 {
			width: 27.5rem;
		}

		.panel .span-3 {
			width: 30rem;
		}

		.panel .span-3-25 {
			width: 32.5rem;
		}

		.panel .span-3-5 {
			width: 35rem;
		}

		.panel .span-3-75 {
			width: 37.5rem;
		}

		.panel .span-4 {
			width: 40rem;
		}

		.panel .span-4-25 {
			width: 42.5rem;
		}

		.panel .span-4-5 {
			width: 45rem;
		}

		.panel .span-4-75 {
			width: 47.5rem;
		}

		.panel .span-5 {
			width: 50rem;
		}

		.panel .span-5-25 {
			width: 52.5rem;
		}

		.panel .span-5-5 {
			width: 55rem;
		}

		.panel .span-5-75 {
			width: 57.5rem;
		}

		.panel .span-6 {
			width: 60rem;
		}

		.panel .span-6-25 {
			width: 62.5rem;
		}

		.panel .span-6-5 {
			width: 65rem;
		}

		.panel .span-6-75 {
			width: 67.5rem;
		}

		.panel .span-7 {
			width: 70rem;
		}

		.panel .span-7-25 {
			width: 72.5rem;
		}

		.panel .span-7-5 {
			width: 75rem;
		}

		.panel .span-7-75 {
			width: 77.5rem;
		}

		.panel .span-8 {
			width: 80rem;
		}

		.panel .span-8-25 {
			width: 82.5rem;
		}

		.panel .span-8-5 {
			width: 85rem;
		}

		.panel .span-8-75 {
			width: 87.5rem;
		}

		.panel .span-9 {
			width: 90rem;
		}

		.panel .span-9-25 {
			width: 92.5rem;
		}

		.panel .span-9-5 {
			width: 95rem;
		}

		.panel .span-9-75 {
			width: 97.5rem;
		}

		.panel .span-10 {
			width: 100rem;
		}

		.panel.small {
			width: 35rem;
		}

		.panel.medium {
			width: 50rem;
		}

		.panel.large {
			width: 65rem;
		}

		.panel.small .span-0-25, .panel.medium .span-0-25, .panel.large .span-0-25 {
			width: 2.5%;
		}

		.panel.small .span-0-5, .panel.medium .span-0-5, .panel.large .span-0-5 {
			width: 5%;
		}

		.panel.small .span-0-75, .panel.medium .span-0-75, .panel.large .span-0-75 {
			width: 7.5%;
		}

		.panel.small .span-1, .panel.medium .span-1, .panel.large .span-1 {
			width: 10%;
		}

		.panel.small .span-1-25, .panel.medium .span-1-25, .panel.large .span-1-25 {
			width: 12.5%;
		}

		.panel.small .span-1-5, .panel.medium .span-1-5, .panel.large .span-1-5 {
			width: 15%;
		}

		.panel.small .span-1-75, .panel.medium .span-1-75, .panel.large .span-1-75 {
			width: 17.5%;
		}

		.panel.small .span-2, .panel.medium .span-2, .panel.large .span-2 {
			width: 20%;
		}

		.panel.small .span-2-25, .panel.medium .span-2-25, .panel.large .span-2-25 {
			width: 22.5%;
		}

		.panel.small .span-2-5, .panel.medium .span-2-5, .panel.large .span-2-5 {
			width: 25%;
		}

		.panel.small .span-2-75, .panel.medium .span-2-75, .panel.large .span-2-75 {
			width: 27.5%;
		}

		.panel.small .span-3, .panel.medium .span-3, .panel.large .span-3 {
			width: 30%;
		}

		.panel.small .span-3-25, .panel.medium .span-3-25, .panel.large .span-3-25 {
			width: 32.5%;
		}

		.panel.small .span-3-5, .panel.medium .span-3-5, .panel.large .span-3-5 {
			width: 35%;
		}

		.panel.small .span-3-75, .panel.medium .span-3-75, .panel.large .span-3-75 {
			width: 37.5%;
		}

		.panel.small .span-4, .panel.medium .span-4, .panel.large .span-4 {
			width: 40%;
		}

		.panel.small .span-4-25, .panel.medium .span-4-25, .panel.large .span-4-25 {
			width: 42.5%;
		}

		.panel.small .span-4-5, .panel.medium .span-4-5, .panel.large .span-4-5 {
			width: 45%;
		}

		.panel.small .span-4-75, .panel.medium .span-4-75, .panel.large .span-4-75 {
			width: 47.5%;
		}

		.panel.small .span-5, .panel.medium .span-5, .panel.large .span-5 {
			width: 50%;
		}

		.panel.small .span-5-25, .panel.medium .span-5-25, .panel.large .span-5-25 {
			width: 52.5%;
		}

		.panel.small .span-5-5, .panel.medium .span-5-5, .panel.large .span-5-5 {
			width: 55%;
		}

		.panel.small .span-5-75, .panel.medium .span-5-75, .panel.large .span-5-75 {
			width: 57.5%;
		}

		.panel.small .span-6, .panel.medium .span-6, .panel.large .span-6 {
			width: 60%;
		}

		.panel.small .span-6-25, .panel.medium .span-6-25, .panel.large .span-6-25 {
			width: 62.5%;
		}

		.panel.small .span-6-5, .panel.medium .span-6-5, .panel.large .span-6-5 {
			width: 65%;
		}

		.panel.small .span-6-75, .panel.medium .span-6-75, .panel.large .span-6-75 {
			width: 67.5%;
		}

		.panel.small .span-7, .panel.medium .span-7, .panel.large .span-7 {
			width: 70%;
		}

		.panel.small .span-7-25, .panel.medium .span-7-25, .panel.large .span-7-25 {
			width: 72.5%;
		}

		.panel.small .span-7-5, .panel.medium .span-7-5, .panel.large .span-7-5 {
			width: 75%;
		}

		.panel.small .span-7-75, .panel.medium .span-7-75, .panel.large .span-7-75 {
			width: 77.5%;
		}

		.panel.small .span-8, .panel.medium .span-8, .panel.large .span-8 {
			width: 80%;
		}

		.panel.small .span-8-25, .panel.medium .span-8-25, .panel.large .span-8-25 {
			width: 82.5%;
		}

		.panel.small .span-8-5, .panel.medium .span-8-5, .panel.large .span-8-5 {
			width: 85%;
		}

		.panel.small .span-8-75, .panel.medium .span-8-75, .panel.large .span-8-75 {
			width: 87.5%;
		}

		.panel.small .span-9, .panel.medium .span-9, .panel.large .span-9 {
			width: 90%;
		}

		.panel.small .span-9-25, .panel.medium .span-9-25, .panel.large .span-9-25 {
			width: 92.5%;
		}

		.panel.small .span-9-5, .panel.medium .span-9-5, .panel.large .span-9-5 {
			width: 95%;
		}

		.panel.small .span-9-75, .panel.medium .span-9-75, .panel.large .span-9-75 {
			width: 97.5%;
		}

		.panel.small .span-10, .panel.medium .span-10, .panel.large .span-10 {
			width: 100%;
		}

		.panel.color0 {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, #726193 20%, #e37b7c 60%, #ffe4b4);
			background-size: 128px 128px, auto;
		}

		.panel.color1 {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
			background-size: 128px 128px, auto;
			background-color: #726193;
		}

		.panel.color2 {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
			background-size: 128px 128px, auto;
			background-color: #e37b7c;
		}

		.panel.color3 {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
			background-size: 128px 128px, auto;
			background-color: #ffe4b4;
		}

		.panel.color4 {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
			background-size: 128px 128px, auto;
			background-color: #353865;
		}

		.panel.color1-alt {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
			background-size: 128px 128px, auto;
			background-color: #6c5e86;
		}

		.panel.color2-alt {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
			background-size: 128px 128px, auto;
			background-color: #de7172;
		}

		.panel.color3-alt {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
			background-size: 128px 128px, auto;
			background-color: #fedea6;
		}

		.panel.color4-alt {
			background-image: url("../../images/overlay.png"), linear-gradient(45deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
			background-size: 128px 128px, auto;
			background-color: #323459;
		}

	@media screen and (max-width: 736px) {

		.panel {
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			height: auto;
		}

			.panel > *.color1 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #726193;
			}

			.panel > *.color2 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #e37b7c;
			}

			.panel > *.color3 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #ffe4b4;
			}

			.panel > *.color4 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #353865;
			}

			.panel > *.color1-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #6c5e86;
			}

			.panel > *.color2-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #de7172;
			}

			.panel > *.color3-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #fedea6;
			}

			.panel > *.color4-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #323459;
			}

			.panel > .intro {
				padding: 2.8875rem 1.75rem 1.3875rem 1.75rem ;
				width: 100% !important;
			}

				.panel > .intro.joined {
					padding-bottom: 0;
					padding-right: 1.75rem;
				}

					.panel > .intro.joined + .inner {
						padding-top: 0;
						padding-left: 1.75rem;
					}

			.panel > .inner {
				padding: 2.8875rem 1.75rem 1.3875rem 1.75rem ;
			}

				.panel > .inner.columns {
					-moz-flex-direction: column;
					-webkit-flex-direction: column;
					-ms-flex-direction: column;
					flex-direction: column;
				}

					.panel > .inner.columns > * {
						margin-left: 0;
						margin-top: 0;
					}

					.panel > .inner.columns > :first-child {
						margin-top: 0;
					}

					.panel > .inner.columns.divided > * {
						margin-left: 0;
						margin-top: 3.5rem;
					}

						.panel > .inner.columns.divided > *:before {
							content: '';
							position: absolute;
							top: auto;
							left: 1.75rem;
							width: calc(100% - 3.5rem);
							height: 2px;
							margin-left: 0;
							margin-top: -1.75rem;
						}

					.panel > .inner.columns.divided > :first-child {
						margin-top: 0;
					}

			.panel .span-0-25 {
				width: 100%;
			}

			.panel .span-0-5 {
				width: 100%;
			}

			.panel .span-0-75 {
				width: 100%;
			}

			.panel .span-1 {
				width: 100%;
			}

			.panel .span-1-25 {
				width: 100%;
			}

			.panel .span-1-5 {
				width: 100%;
			}

			.panel .span-1-75 {
				width: 100%;
			}

			.panel .span-2 {
				width: 100%;
			}

			.panel .span-2-25 {
				width: 100%;
			}

			.panel .span-2-5 {
				width: 100%;
			}

			.panel .span-2-75 {
				width: 100%;
			}

			.panel .span-3 {
				width: 100%;
			}

			.panel .span-3-25 {
				width: 100%;
			}

			.panel .span-3-5 {
				width: 100%;
			}

			.panel .span-3-75 {
				width: 100%;
			}

			.panel .span-4 {
				width: 100%;
			}

			.panel .span-4-25 {
				width: 100%;
			}

			.panel .span-4-5 {
				width: 100%;
			}

			.panel .span-4-75 {
				width: 100%;
			}

			.panel .span-5 {
				width: 100%;
			}

			.panel .span-5-25 {
				width: 100%;
			}

			.panel .span-5-5 {
				width: 100%;
			}

			.panel .span-5-75 {
				width: 100%;
			}

			.panel .span-6 {
				width: 100%;
			}

			.panel .span-6-25 {
				width: 100%;
			}

			.panel .span-6-5 {
				width: 100%;
			}

			.panel .span-6-75 {
				width: 100%;
			}

			.panel .span-7 {
				width: 100%;
			}

			.panel .span-7-25 {
				width: 100%;
			}

			.panel .span-7-5 {
				width: 100%;
			}

			.panel .span-7-75 {
				width: 100%;
			}

			.panel .span-8 {
				width: 100%;
			}

			.panel .span-8-25 {
				width: 100%;
			}

			.panel .span-8-5 {
				width: 100%;
			}

			.panel .span-8-75 {
				width: 100%;
			}

			.panel .span-9 {
				width: 100%;
			}

			.panel .span-9-25 {
				width: 100%;
			}

			.panel .span-9-5 {
				width: 100%;
			}

			.panel .span-9-75 {
				width: 100%;
			}

			.panel .span-10 {
				width: 100%;
			}

			.panel.small, .panel.medium, .panel.large {
				width: 100% !important;
			}

				.panel.small .span-0-25, .panel.medium .span-0-25, .panel.large .span-0-25 {
					width: 100%;
				}

				.panel.small .span-0-5, .panel.medium .span-0-5, .panel.large .span-0-5 {
					width: 100%;
				}

				.panel.small .span-0-75, .panel.medium .span-0-75, .panel.large .span-0-75 {
					width: 100%;
				}

				.panel.small .span-1, .panel.medium .span-1, .panel.large .span-1 {
					width: 100%;
				}

				.panel.small .span-1-25, .panel.medium .span-1-25, .panel.large .span-1-25 {
					width: 100%;
				}

				.panel.small .span-1-5, .panel.medium .span-1-5, .panel.large .span-1-5 {
					width: 100%;
				}

				.panel.small .span-1-75, .panel.medium .span-1-75, .panel.large .span-1-75 {
					width: 100%;
				}

				.panel.small .span-2, .panel.medium .span-2, .panel.large .span-2 {
					width: 100%;
				}

				.panel.small .span-2-25, .panel.medium .span-2-25, .panel.large .span-2-25 {
					width: 100%;
				}

				.panel.small .span-2-5, .panel.medium .span-2-5, .panel.large .span-2-5 {
					width: 100%;
				}

				.panel.small .span-2-75, .panel.medium .span-2-75, .panel.large .span-2-75 {
					width: 100%;
				}

				.panel.small .span-3, .panel.medium .span-3, .panel.large .span-3 {
					width: 100%;
				}

				.panel.small .span-3-25, .panel.medium .span-3-25, .panel.large .span-3-25 {
					width: 100%;
				}

				.panel.small .span-3-5, .panel.medium .span-3-5, .panel.large .span-3-5 {
					width: 100%;
				}

				.panel.small .span-3-75, .panel.medium .span-3-75, .panel.large .span-3-75 {
					width: 100%;
				}

				.panel.small .span-4, .panel.medium .span-4, .panel.large .span-4 {
					width: 100%;
				}

				.panel.small .span-4-25, .panel.medium .span-4-25, .panel.large .span-4-25 {
					width: 100%;
				}

				.panel.small .span-4-5, .panel.medium .span-4-5, .panel.large .span-4-5 {
					width: 100%;
				}

				.panel.small .span-4-75, .panel.medium .span-4-75, .panel.large .span-4-75 {
					width: 100%;
				}

				.panel.small .span-5, .panel.medium .span-5, .panel.large .span-5 {
					width: 100%;
				}

				.panel.small .span-5-25, .panel.medium .span-5-25, .panel.large .span-5-25 {
					width: 100%;
				}

				.panel.small .span-5-5, .panel.medium .span-5-5, .panel.large .span-5-5 {
					width: 100%;
				}

				.panel.small .span-5-75, .panel.medium .span-5-75, .panel.large .span-5-75 {
					width: 100%;
				}

				.panel.small .span-6, .panel.medium .span-6, .panel.large .span-6 {
					width: 100%;
				}

				.panel.small .span-6-25, .panel.medium .span-6-25, .panel.large .span-6-25 {
					width: 100%;
				}

				.panel.small .span-6-5, .panel.medium .span-6-5, .panel.large .span-6-5 {
					width: 100%;
				}

				.panel.small .span-6-75, .panel.medium .span-6-75, .panel.large .span-6-75 {
					width: 100%;
				}

				.panel.small .span-7, .panel.medium .span-7, .panel.large .span-7 {
					width: 100%;
				}

				.panel.small .span-7-25, .panel.medium .span-7-25, .panel.large .span-7-25 {
					width: 100%;
				}

				.panel.small .span-7-5, .panel.medium .span-7-5, .panel.large .span-7-5 {
					width: 100%;
				}

				.panel.small .span-7-75, .panel.medium .span-7-75, .panel.large .span-7-75 {
					width: 100%;
				}

				.panel.small .span-8, .panel.medium .span-8, .panel.large .span-8 {
					width: 100%;
				}

				.panel.small .span-8-25, .panel.medium .span-8-25, .panel.large .span-8-25 {
					width: 100%;
				}

				.panel.small .span-8-5, .panel.medium .span-8-5, .panel.large .span-8-5 {
					width: 100%;
				}

				.panel.small .span-8-75, .panel.medium .span-8-75, .panel.large .span-8-75 {
					width: 100%;
				}

				.panel.small .span-9, .panel.medium .span-9, .panel.large .span-9 {
					width: 100%;
				}

				.panel.small .span-9-25, .panel.medium .span-9-25, .panel.large .span-9-25 {
					width: 100%;
				}

				.panel.small .span-9-5, .panel.medium .span-9-5, .panel.large .span-9-5 {
					width: 100%;
				}

				.panel.small .span-9-75, .panel.medium .span-9-75, .panel.large .span-9-75 {
					width: 100%;
				}

				.panel.small .span-10, .panel.medium .span-10, .panel.large .span-10 {
					width: 100%;
				}

			.panel.color1 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #726193;
			}

			.panel.color2 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #e37b7c;
			}

			.panel.color3 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #ffe4b4;
			}

			.panel.color4 {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.25) 25%, rgba(227, 123, 124, 0.25) 50%, rgba(255, 228, 180, 0.25));
				background-size: 128px 128px, auto;
				background-color: #353865;
			}

			.panel.color1-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #6c5e86;
			}

			.panel.color2-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #de7172;
			}

			.panel.color3-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #fedea6;
			}

			.panel.color4-alt {
				background-image: url("../../images/overlay.png"), linear-gradient(135deg, rgba(114, 97, 147, 0.175) 25%, rgba(227, 123, 124, 0.175) 50%, rgba(255, 228, 180, 0.175));
				background-size: 128px 128px, auto;
				background-color: #323459;
			}

	}

/* Panel (Banner) */

	.panel.banner {
		-moz-align-items: stretch;
		-webkit-align-items: stretch;
		-ms-align-items: stretch;
		align-items: stretch;
	}

		.panel.banner .content {
			padding: 3.5rem 3.5rem 2rem 3.5rem ;
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			-moz-flex-grow: 0;
			-webkit-flex-grow: 0;
			-ms-flex-grow: 0;
			flex-grow: 0;
			-moz-flex-shrink: 0;
			-webkit-flex-shrink: 0;
			-ms-flex-shrink: 0;
			flex-shrink: 0;
		}

			.panel.banner .content > .actions:last-child {
				margin-bottom: 0;
			}

		.panel.banner .image {
			-moz-flex-grow: 0;
			-webkit-flex-grow: 0;
			-ms-flex-grow: 0;
			flex-grow: 0;
			-moz-flex-shrink: 0;
			-webkit-flex-shrink: 0;
			-ms-flex-shrink: 0;
			flex-shrink: 0;
			position: relative;
		}

			.panel.banner .image img {
				-moz-object-fit: cover;
				-webkit-object-fit: cover;
				-ms-object-fit: cover;
				object-fit: cover;
				display: block;
				position: absolute;
				top: 0;
				left: 0;
				width: 100%;
				height: 100%;
			}

		.panel.banner.left {
			-moz-flex-direction: row;
			-webkit-flex-direction: row;
			-ms-flex-direction: row;
			flex-direction: row;
		}

		.panel.banner.right {
			-moz-flex-direction: row-reverse;
			-webkit-flex-direction: row-reverse;
			-ms-flex-direction: row-reverse;
			flex-direction: row-reverse;
		}

	@media screen and (max-width: 736px) {

		.panel.banner .content {
			padding: 2.8875rem 1.75rem 1.3875rem 1.75rem ;
			-moz-flex-basis: 60%;
			-webkit-flex-basis: 60%;
			-ms-flex-basis: 60%;
			flex-basis: 60%;
		}

			.panel.banner .content > .actions:last-child {
				margin-bottom: 1.5rem;
			}

		.panel.banner .image {
			-moz-flex-basis: 40%;
			-webkit-flex-basis: 40%;
			-ms-flex-basis: 40%;
			flex-basis: 40%;
		}

	}

	@media screen and (max-width: 736px) and (orientation: portrait) {

		.panel.banner .content {
			-moz-flex-basis: auto;
			-webkit-flex-basis: auto;
			-ms-flex-basis: auto;
			flex-basis: auto;
		}

		.panel.banner .image {
			-moz-flex-basis: auto;
			-webkit-flex-basis: auto;
			-ms-flex-basis: auto;
			flex-basis: auto;
			height: 18rem;
		}

		.panel.banner.left {
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
		}

		.panel.banner.right {
			-moz-flex-direction: column-reverse;
			-webkit-flex-direction: column-reverse;
			-ms-flex-direction: column-reverse;
			flex-direction: column-reverse;
		}

	}

/* Panel (Spotlight) */

	.panel.spotlight {
		-moz-align-items: stretch;
		-webkit-align-items: stretch;
		-ms-align-items: stretch;
		align-items: stretch;
		position: relative;
	}

		.panel.spotlight > * {
			z-index: 1;
		}

		.panel.spotlight .content {
			display: -moz-flex;
			display: -webkit-flex;
			display: -ms-flex;
			display: flex;
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			-moz-justify-content: center;
			-webkit-justify-content: center;
			-ms-justify-content: center;
			justify-content: center;
			padding: 3.5rem 3.5rem 2rem 3.5rem ;
		}

		.panel.spotlight .image {
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 100%;
			z-index: 0;
		}

			.panel.spotlight .image img {
				-moz-object-fit: cover;
				-webkit-object-fit: cover;
				-ms-object-fit: cover;
				object-fit: cover;
				display: block;
				position: absolute;
				top: 0;
				left: 0;
				width: 100%;
				height: 100%;
			}

		.panel.spotlight.left {
			-moz-justify-content: -moz-flex-start;
			-webkit-justify-content: -webkit-flex-start;
			-ms-justify-content: -ms-flex-start;
			justify-content: flex-start;
		}

			.panel.spotlight.left .content {
				background-image: linear-gradient(-90deg, transparent 0%, rgba(0, 0, 0, 0.125) 30%, rgba(0, 0, 0, 0.175) 50%);
			}

		.panel.spotlight.right {
			-moz-justify-content: -moz-flex-end;
			-webkit-justify-content: -webkit-flex-end;
			-ms-justify-content: -ms-flex-end;
			justify-content: flex-end;
		}

			.panel.spotlight.right .content {
				background-image: linear-gradient(90deg, transparent 0%, rgba(0, 0, 0, 0.125) 30%, rgba(0, 0, 0, 0.175) 50%);
			}

	@media screen and (max-width: 736px) {

		.panel.spotlight .content {
			padding: 2.8875rem 1.75rem 1.3875rem 1.75rem ;
			-moz-flex-direction: column !important;
			-webkit-flex-direction: column !important;
			-ms-flex-direction: column !important;
			flex-direction: column !important;
			background-image: linear-gradient(0deg, rgba(0, 0, 0, 0.25) 70%, rgba(0, 0, 0, 0.175)) !important;
			min-height: 25rem;
		}

	}

	@media screen and (max-width: 480px) {

		.panel.spotlight .content {
			min-height: 30rem;
		}

	}

/* Page Wrapper */

	#page-wrapper {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-align-items: center;
		-webkit-align-items: center;
		-ms-align-items: center;
		align-items: center;
		-moz-justify-content: -moz-flex-start;
		-webkit-justify-content: -webkit-flex-start;
		-ms-justify-content: -ms-flex-start;
		justify-content: flex-start;
		-moz-flex-grow: 1;
		-webkit-flex-grow: 1;
		-ms-flex-grow: 1;
		flex-grow: 1;
		-moz-flex-shrink: 1;
		-webkit-flex-shrink: 1;
		-ms-flex-shrink: 1;
		flex-shrink: 1;
		height: 100%;
		padding: 5rem;
	}

		@media screen and (orientation: portrait) {

			#page-wrapper {
				padding-left: 2rem;
				padding-right: 2rem;
			}

		}

		@media screen and (min-aspect-ratio: 16 / 7) {

			#page-wrapper {
				padding: 6vh;
			}

		}

		@media screen and (min-aspect-ratio: 16 / 6) {

			#page-wrapper {
				padding: 0;
			}

		}

	@media screen and (max-width: 736px) {

		#page-wrapper {
			height: auto;
			padding: 1rem;
		}

	}

	@media screen and (max-width: 480px) {

		#page-wrapper {
			padding: 0;
		}

	}

/* Wrapper */

	#wrapper {
		display: -moz-flex;
		display: -webkit-flex;
		display: -ms-flex;
		display: flex;
		-moz-flex-direction: row;
		-webkit-flex-direction: row;
		-ms-flex-direction: row;
		flex-direction: row;
		-moz-transition: opacity 1s ease-out, -moz-transform 0.75s ease-out;
		-webkit-transition: opacity 1s ease-out, -webkit-transform 0.75s ease-out;
		-ms-transition: opacity 1s ease-out, -ms-transform 0.75s ease-out;
		transition: opacity 1s ease-out, transform 0.75s ease-out;
		-moz-transition-delay: 0.25s;
		-webkit-transition-delay: 0.25s;
		-ms-transition-delay: 0.25s;
		transition-delay: 0.25s;
		cursor: default;
		position: relative;
		height: 32rem;
		box-shadow: 0 2rem 4rem 0.25rem rgba(46, 43, 55, 0.575);
	}

		#wrapper > .scrollZone {
			position: fixed;
			width: 6rem;
			height: inherit;
			cursor: -moz-grab;
			cursor: -webkit-grab;
			cursor: -ms-grab;
			cursor: grab;
			z-index: 10100;
		}

			#wrapper > .scrollZone.left {
				left: 0;
			}

			#wrapper > .scrollZone.right {
				right: 0;
			}

		#wrapper > .copyright {
			position: absolute;
			bottom: -3rem;
			right: 0;
			font-size: 0.8rem;
			color: rgba(46, 43, 55, 0.375);
			margin-bottom: 0;
		}

			#wrapper > .copyright a:hover {
				color: inherit;
			}

		#wrapper.is-dragging {
			-moz-user-select: none;
			-webkit-user-select: none;
			-ms-user-select: none;
			user-select: none;
			cursor: -moz-grab;
			cursor: -webkit-grab;
			cursor: -ms-grab;
			cursor: grab;
		}

			#wrapper.is-dragging * {
				-moz-user-select: none;
				-webkit-user-select: none;
				-ms-user-select: none;
				user-select: none;
			}

			#wrapper.is-dragging *:not(a, .image) {
				cursor: -moz-grab;
				cursor: -webkit-grab;
				cursor: -ms-grab;
				cursor: grab;
			}

		#wrapper.is-dragged * {
			-moz-pointer-events: none;
			-webkit-pointer-events: none;
			-ms-pointer-events: none;
			pointer-events: none;
		}

		body.is-loading #wrapper {
			-moz-transform: translateX(2rem);
			-webkit-transform: translateX(2rem);
			-ms-transform: translateX(2rem);
			transform: translateX(2rem);
			opacity: 0;
		}

	@media screen and (max-width: 736px) {

		#wrapper {
			-moz-flex-direction: column;
			-webkit-flex-direction: column;
			-ms-flex-direction: column;
			flex-direction: column;
			height: auto;
			margin: 0 0 5rem 0;
			box-shadow: 0 0.25rem 1.5rem 0.25rem rgba(46, 43, 55, 0.5);
		}

			#wrapper > .scrollZone {
				display: none;
			}

			#wrapper > .copyright {
				display: block;
				width: 100%;
				text-align: center;
			}

			body.is-loading #wrapper {
				-moz-transform: translateY(1rem);
				-webkit-transform: translateY(1rem);
				-ms-transform: translateY(1rem);
				transform: translateY(1rem);
			}

	}

	@media screen and (max-width: 480px) {

		#wrapper {
			box-shadow: none;
		}

			body.is-loading #wrapper {
				-moz-transform: none;
				-webkit-transform: none;
				-ms-transform: none;
				transform: none;
			}

	}
