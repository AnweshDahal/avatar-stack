# Card Avatar Stack

_By [Anwesh Dahal](http://github.com/AnweshDahal)_

![](https://img.shields.io/badge/Sass-CC6699?style=for-the-badge&logo=sass&logoColor=white)

This is a simple SASS/SCSS plugin to display user avatars, _primarily in cards_,

## Installation

1. Download the repository and copy the `_avatars.scss` to your scss directory
2. import the avatar using `@import "avatars";`

## Adding the Avatar Stack to a card

Though the stack is intended for a card, you can use this plugin in any component.

### HTML

Insert the following code inside a card

```html
<div class="card">
	<div class="card-header">
		...
		<div class="avatars">
			<!-- You use it with just an image file -->
			<img src"..." class="avatar"/>
			<!-- Or in an <a> tag with the image inside -->
			<a href="..." class="avatar">
				<img src="..." />
			</a>
		</div>
	</div>
</div>
```

### SASS

```scss
@import "avatar";
```

## Customizing the stack

You can customize the style as much as you like however, if you want to change only the basic stuff you can do so by modifying the variable on top.

```scss
$avatar-border: #fff;
$avatar-width: 1.85rem; // ~30px
$avatar-container-width: 160px;
```

After some testings I found that keeping the `avatar-container-width` to approximately ~80% of the parent container works best, but you can set it as you want.
