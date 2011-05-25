# Base CSS

This is just a CSS stylesheet I start all of my projects with. It includes some handy classes and rules that I commonly use, along with a simple reset to keep things consistent.

Below are just a few basic pieces of code showing how some of the classes work, the rest is pretty self-explanatory by looking through the CSS file.

## Notices

	<div class="notice info">
		<p>This is just a <strong>simple</strong> notification. It can container whatever you'd like.</p>
		<a href="#" class="close">&times;</a>
	</div>

## Forms

Using `ul.fields` gives you an easy way to layout complex forms without using tables.

As you'll see, each `<li>` is a row, and each `<div>` is basically a cell (a floated `<div>`).

	<ul class="fields">
		<li>
			<div>
				<label for="firstname">First Name:</label>
				<input name="firstname" id="firstname" class="input" />
			</div>
			<div>
				<label for="lastname">Last Name:</label>
				<input name="lastname" id="lastname" class="input" />
			</div>
			<div>
				<label for="nickname">Nickname:</label>
				<input name="nickname" id="nickname" class="input" />
			</div>
		</li>
		<li>
			<div>
				<label for="age" class="inline">Age:</label> 
				<input type="number" name="age" id="age" class="input" />
				<small>Enter your current age. Example: "20"</small>
			</div>
		</li>
		<li class="divider">
			<div>
				<h2>Section Title</h2>
			</div>
		</li>
		<li>
			<div>
				<button class="large red">Submit Form!</button>
			</div>
		</li>
	</ul>