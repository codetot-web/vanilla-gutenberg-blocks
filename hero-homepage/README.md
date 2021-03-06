# Hero Homepage

## Tested with:

- Theme: GeneratePress

## Fields
- Title
- Description
- Button Text
- Mobile Image
- Desktop Image

## Markup

```
<!-- wp:group {"className":"ct-hero-homepage"} -->
<div class="wp-block-group ct-hero-homepage"><div class="wp-block-group__inner-container"><!-- wp:html -->
<div class="ct-hero-homepage__svg"><svg viewBox="0 0 587 715" fill="none"><g clip-path="url(#blob-right-large_svg__clip0)"><path fill="#fff" d="M0 0h587v715H0z"></path><path d="M488.441 714.015c-134.937 0-125.246-126.527-385.233-84.099C-156.778 672.343 119.465-15.873 420.505.059c301.04 15.932 163.537 228.416 257.323 384.666 93.785 156.25-54.45 329.29-189.387 329.29z" fill="#F3F1FE"></path></g><defs><clipPath id="blob-right-large_svg__clip0"><path fill="#fff" d="M0 0h587v715H0z"></path></clipPath></defs></svg></div>
<!-- /wp:html -->

<!-- wp:group {"className":"ct-hero-homepage__content"} -->
<div class="wp-block-group ct-hero-homepage__content"><div class="wp-block-group__inner-container"><!-- wp:heading {"className":"ct-hero-homepage__title"} -->
<h2 class="ct-hero-homepage__title">Dịch vụ phát triển website trọn gói</h2>
<!-- /wp:heading -->

<!-- wp:paragraph {"className":"ct-hero-homepage__description"} -->
<p class="ct-hero-homepage__description">Xây dựng website theo tiêu chuẩn quốc tế, hỗ trợ tối đa khả năng mở rộng.</p>
<!-- /wp:paragraph -->

<!-- wp:buttons -->
<div class="wp-block-buttons"><!-- wp:button {"borderRadius":0,"backgroundColor":"vivid-cyan-blue","textColor":"white","className":"is-style-fill ct-hero-homepage__button"} -->
<div class="wp-block-button is-style-fill ct-hero-homepage__button"><a class="wp-block-button__link has-white-color has-vivid-cyan-blue-background-color has-text-color has-background no-border-radius">Đăng ký dùng thử</a></div>
<!-- /wp:button --></div>
<!-- /wp:buttons --></div></div>
<!-- /wp:group -->

<!-- wp:group {"className":"ct-hero-homepage__images"} -->
<div class="wp-block-group ct-hero-homepage__images"><div class="wp-block-group__inner-container"><!-- wp:image {"id":26,"width":179,"height":179,"sizeSlug":"full","linkDestination":"none","className":"ct-hero-homepage__mobile-image"} -->
<figure class="wp-block-image size-full is-resized ct-hero-homepage__mobile-image"><img src="https://placeimg.com/179/179/tech/grayscale" alt="Mobile  view" class="wp-image-26" width="179" height="179"/></figure>
<!-- /wp:image -->

<!-- wp:image {"id":27,"width":1438,"height":787,"sizeSlug":"full","linkDestination":"none","className":"ct-hero-homepage__desktop-image"} -->
<figure class="wp-block-image size-full is-resized ct-hero-homepage__desktop-image"><img src="https://placeimg.com/1000/700/tech/grayscale" alt="" class="wp-image-27" width="1438" height="787" title=""/></figure>
<!-- /wp:image --></div></div>
<!-- /wp:group --></div></div>
<!-- /wp:group -->
```

## Stylesheet

.ct-hero-homepage {
  position: relative;
  background: #fff;
  overflow: hidden;
}

.ct-hero-homepage__svg {
  position: absolute;
  top: 0;
  right: 0;
  width: 35%;
}

.ct-hero-homepage__content,
.ct-hero-homepage__images {
  position: relative;
  z-index: 2;
}

.ct-hero-homepage > .wp-block-group__inner-container {
	max-width: 100%;
	margin: 0;
}

.ct-hero-homepage__images > .wp-block-group__inner-container {
  position: relative;
  width: 100%;
}

.ct-hero-homepage__mobile-image {
  position: absolute;
  top: calc(50% + 40px);
  left: 0;
  width: 240px;
  z-index: 2;
  transform: translateY(-50%);
}

.ct-hero-homepage__mobile-image,
.ct-hero-homepage__desktop-image {
  display: inline-flex;
  margin: 0;
}

.ct-hero-homepage__title {
  font-weight: 700;
}

.ct-hero-homepage__content > .wp-block-group__inner-container {
	padding-left: 0;
	padding-right: 0;
}

@media screen and (min-width: 1024px) {
	.ct-hero-homepage > .wp-block-group__inner-container {
		display: flex;
    max-width: 1200px;
    margin: 0 auto;
	}
	
	.ct-hero-homepage__content {
	  display: flex;
    align-items: center;
	  width: 45%;
    min-height: 600px;
  }
  
  .ct-hero-homepage__content > .wp-block-group__inner-container {
    max-width: 45vh;
    margin: 0;
    padding: 0;
  }
	
	.ct-hero-homepage__images {
		width: 55%;
    display: flex;
    align-items: center;
	}
}

@media screen and (min-width: 1280px) {
  .ct-hero-homepage__title {
    font-size: 3rem;
  }
}
