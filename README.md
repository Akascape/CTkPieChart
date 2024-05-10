# CTkPieChart
Another piece in the puzzle, pie chart widget for customtkinter, simple and easy to visualize any data in pie chart form.
## Installation
### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkPieChart?&color=white&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/CTkPieChart/archive/refs/heads/main.zip)

Download the source code, paste the `CTkPieChart` folder in the directory where your program is present.

## Usage
```python
import customtkinter
```

## Arguments
| Parameters | Details |
|--------|----------|
| master	| root window, can be _CTk_ or _CTkFrame_|
| radius | the initial size of the pie chart |
| line_width | size of the inner radius |
| border_width | add border around the pie chart |
| border_color | color of the borders |
| bg_color | background color of the widget |
| text_color | color of the label text |

## Methods
- **.add(tag, value, color, text_color)**: adds new data in the chart, **tag**: section name; **data**: value; **color**: color of section (optional, choses color randomly by default), **text_color**: color of text over the section (optional)
- **.delete(tag)**: delete a section from the chart
- **.update(tag, *args)**: update any tag data
- **.get(tag)**: return data/color of the chart sections, tag is optional
- **.configure(*args)**: change parameters of the pie chart
- **.cget(parameter)**: return the required parameter from the chart

Follow me for more stuff like this: [`Akascape`](https://github.com/Akascape/)
### That's all, hope it will help!

