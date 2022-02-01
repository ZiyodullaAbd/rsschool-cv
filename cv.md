#### Personal data

<!-- Name: **Ziyodulla**
Surname: **Abdurakhmonov**
Date of birth: **27.01.2004** -->
<div style="display:flex;align-items:center;justify-content:space-between;">
    <div>
        <p style="margin-bottom: 5px"><b>Name: </b>Ziyodulla</p>
        <p style="margin-bottom: 5px"><b>Surname: </b>Abdurakhmonov</p>
        <p style="margin-bottom: 5px"><b>Date of birth:</b> 27.01.2004</p>
        <p style="margin-bottom: 5px"><b>Residence: </b>Uzbekistan, Tashkent</p>
        <p style="margin-bottom: 5px"><b>Nationality: </b>Uzbek</p>
    </div>
    <img alt="personal photo" src="./images/personal_photo.JPG" width="100px"/>
</div>

##### About myself
I am a hardworking, ambitious and responsible full-stack web developer from Uzbekistan who always tries to learn something new. I can learn new technologies as well as skills quickly. I am excellent at working with a team and while working in a team I always try to get some new knowledge from more experienced team members. I am able to work with pure JavaScript and its framework Vue. As well as this, I can work with CSS preprocessors like SCSS / LESS or CSS libraries like Bootstrap, Tailwind. Also, I can write backend logic using PHP / NodeJs, frameworks like Laravel / ExpressJs and databases like MongoDB / MySql.

***

#### Education

**2010 - 2019:** School № 97
**2019 - 2021:** Academic lyceum under Westminster Internation Universtify in Tashkent
**2021 - now:** Westminster Internation Universtify in Tashkent

***

#### Contact details

Phone number: [+998 (99) 437-41-54](tel:+998994374154)
Email: ziyodulla.epam@gamil.com
Telegram: [@ziyodulla_abd](https://telegram.me/ziyodulla_abd)

***

#### Skills

##### Front-end:
| Tecnology |  |
| --- | --- |
| HTML | :star::star::star::star: |
| CSS | :star::star::star::star: |
| JS | :star::star::star::star: |
| Vue, Vuex, Axios | :star::star::star::star: |

##### Backend:

| Tecnology |  |
| --- | --- |
| PHP | :star::star::star::star: |
| Laravel | :star::star::star::star: |

##### Database:

| Tecnology |  |
| --- | --- |
| MySql | :star::star::star: |

***

#### Projects
Auction: [e-onlinesavdo](https://e-onlinesavdo.uz/)

***

#### Example of code

[Human readable duration format](https://www.codewars.com/kata/52742f58faf5485cae000b9a)

```
const second = 1;
const minute = 60;
const hour = minute * 60;
const day = hour * 24;
const year = 365 * day;
const strings = ["year", "day", "hour", "minute", "second"];

function formatDuration(seconds) {
    if (seconds == 0) return "now";
    const time = [year, day, hour, minute, second];

    const times = get_times(time, seconds)
        .map((item, index) => stringify(item, strings[index]))
        .filter((item) => item);
    let last = "";
    if (times.length > 1) last = times.pop();
    return times.join(", ") + (last ? ` and ${last}` : "");
}

function get_times(time, seconds, times = []) {
    if (seconds == 0) return times;
    const current = Math.floor(seconds / time[0]);
    times.push(current);
    const remainder = seconds - current * time[0];
    time.shift();
    return get_times(time, remainder, times);
}

function stringify(num, str) {
    if (!num) return "";
    return num > 1 ? `${num} ${str}s` : `${num} ${str}`;
}
```
