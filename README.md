# task-11
# Task Eleven - Image Hover Effect

This repository contains two different implementations of an image hover effect. Both approaches cause an image to disappear when hovered over and reappear when the mouse leaves the area, but one is implemented using **JavaScript** and the other using **CSS**.

## Files in this repository:
- `index.html` - JavaScript-based solution
- `style.html` - CSS-based solution

### 1. index.html (JavaScript)

This version uses JavaScript to control the hover behavior. When the mouse hovers over the image, the `display` property is set to `none`, hiding the image. Once the mouse leaves, the `display` property is set back to `block`, making the image reappear.

#### How to Run:

- Open the `index.html` file in any web browser.
- Hover over the image to make it disappear and move the mouse away to make it reappear.


<img id="hoverImage" src="https://www.pexels.com/photo/close-photography-of-red-and-pink-rose-56866/" alt="Sample Image" width="500" height="500">

<script>
    const imgElement = document.getElementById('hoverImage');
    
    imgElement.addEventListener('mouseover', function() {
        imgElement.style.display = 'none';
    });
    
    imgElement.addEventListener('mouseout', function() {
        imgElement.style.display = 'block';
    });
</script>

### 2.style.html (CSS)
This version uses CSS only to achieve the same effect. When the mouse hovers over the image, the `opacity` property is set to `0`, making the image invisible. Once the mouse leaves, the `opacity` returns to `1`, making the image visible again.

#### How to Run:

- Open the `style.html` file in any web browser.
- Hover over the image to see it fade out, and move the mouse away to see it fade back in.

```css
img:hover {
    opacity: 0;
}
