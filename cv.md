
### [rsschool-cv](https://rs.school/)

---
## Yauhen Ranko

### Product owner
---
#### Contact information

Phone: +375 33 385 58 57
E-mail: yauhenranko@gmail.com
Telegram: @YauhenRanko
[![LinkedIn](https://img.icons8.com/?size=100&id=13930&format=png&color=000000)](https://www.linkedin.com/in/yauhen-ranko-63a7801a3/)


---
### Abount Myself:
I have extensive experience in selling IT products. For a long time he was engaged in business analysis in the development of enterprise systems in the field of document management and accounting. I currently hold the position of head of the fintech department.

---
Skill and Proficiency:
* Product Management 
* Sales
* Analytics
* Go 
* Python

---
#### Code example:

Easy function for input float number:

```
package inputfloat

import (
    "bufio"
    "os"
    "strconv"
    "strings"
)

func InputFloat() (float64, error) {
    reader := bufio.NewReader(os.Stdin)
    input, err := reader.ReadString('\n')
    if err != nil {
        return 0, err
    }

    input = strings.TrimSpace(input)
    number, err := strconv.ParseFloat(input, 64)
    if err != nil {
        return 0, err
    }
    return number, nil
}

```

---
#### Courses:
* [Product University](https://productuniversity.ru/)


---
#### Languages:

* English - Intermediate
* Russian - Native
* Germany - Basic


