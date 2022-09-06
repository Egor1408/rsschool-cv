# Prudnikov Egor

## Junior Frontend Developer

---

## Contacts:

-   Phone: +7-920-444-1200
-   E-mail: eguar0886@gmail.com
-   [Telegram](https://tlgg.ru/@Eguar42)
-   [GitHub](https://github.com/Egor1408)

---

## About me

Hello everyone, my name is Egor, I am 36 years old, I come from Novokuznetsk, at the moment I live in Voronezh.

I work as a layout designer, in the junior position, I dream of moving to the position of a JS developer.

I am fond of reading books, roller skating and fishing.

## My Skills

-   HTML5/CSS3 (SCSS)
-   JS (Angular) basic
-   GitHub
-   WebPack, Gulp
-   Figma

---

## Code example:

```
const tabs = (headerSelector, tabSelector, contentSelector, activeClass, display = 'block') => {
    const header = document.querySelector(headerSelector),
        tab = document.querySelectorAll(tabSelector),
        content = document.querySelectorAll(contentSelector);

    function hideTabContent() {
        content.forEach(item => {
            item.style.display = 'none';
        })

        tab.forEach(item => {
            item.classList.remove(activeClass);
        })
    }

    function showTabContent(i = 0) {
        content[i].style.display = display;
        tab[i].classList.add(activeClass);
    }

    hideTabContent();
    showTabContent();

    header.addEventListener('click', (e) => {
        const target = e.target;
        if (target &&
        (target.classList.contains(tabSelector.replace(/\./, "")) ||
        target.parentNode.classList.contains(tabSelector.replace(/\./, "")))) {
            tab.forEach((item, i) => {
                if (target == item || target.parentNode == item) {
                    hideTabContent();
                    showTabContent(i);
                }
            })
        }
    })
};

export default tabs;
```

---

## Courses:

-   [Figma](https://www.udemy.com/course/web-figma-ui/)
-   [HTML5/CSS3](https://htmlacademy.ru/study)
-   [JS LearnJavaScript](https://learn.javascript.ru/)
-   [ReactJS Udemy](https://www.udemy.com/course/react-2020-complete-guide/)
