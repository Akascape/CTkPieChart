# CTkPieChart
Another piece in the puzzle, pie chart widget for customtkinter, simple and easy to visualize any data in pie chart form.

![Screenshot](https://github.com/Akascape/CTkPieChart/assets/89206401/2632a3f0-bf79-40ec-a3a1-bf5252d571b9)

## Features
- Simple widget
- Made specially for customtkinter
- Easily add/configure data
- Chooses color randomly
- Calculates % automatically
- No shart edges in the pie chart

## Installation
### [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkPieChart?&color=white&label=Download%20Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="400">](https://github.com/Akascape/CTkPieChart/archive/refs/heads/main.zip)

Download the source code, paste the `CTkPieChart` folder in the directory where your program is present.

## Usage
```python
import customtkinter
from CTkPieChart import *

root = customtkinter.CTk()

pie_chart = CTkPieChart(root)
pie_chart.pack()
pie_chart.add("A", 10)
pie_chart.add("B", 60, color="cyan", text_color="black")
pie_chart.add("C", 40)

root.mainloop()
```

## Example With Details
```python
from CTkPieChart import *
import customtkinter

root = customtkinter.CTk()

pie_chart = CTkPieChart(root, line_width=50)
pie_chart.pack(side="left", padx=10, pady=10)

pie_chart.add("A", 90)
pie_chart.add("B", 90)
pie_chart.add("C", 90)
pie_chart.add("D", 45)
pie_chart.add("E", 45)

values = pie_chart.get()

frame = customtkinter.CTkFrame(root, fg_color="transparent")
frame.pack(side="left", padx=(0,10), pady=10)

for key, values in values.items():
    data_circle = customtkinter.CTkRadioButton(frame, hover=False, text=key,
                                               width=1,fg_color=values["color"])
    data_circle.select()
    data_circle.pack(pady=5)
    

root.mainloop()
```
![image](https://github.com/Akascape/CTkPieChart/assets/89206401/1b033497-6f99-4994-9540-0c3fffd08cf8)

## Arguments
| Parameters | Details |
|--------|----------|
| master	| root window or frame |
| radius | the initial size of the pie chart |
| line_width | size of the inner radius |
| border_width | add border around the pie chart |
| border_color | color of the borders |
| bg_color | background color of the widget |
| text_color | color of the label text |
| values | add all the values at once, _dict_ |

## Methods
- **.add(tag, value, color, text_color)**: adds new data in the chart, **tag**: section name; **data**: value; **color**: color of section (optional, choses color randomly by default), **text_color**: color of text over the section (optional)
- **.delete(tag)**: delete a section from the chart
- **.update(tag, *args)**: update any tag data
- **.get(tag)**: return data/color of the chart sections, tag is optional
- **.configure(*args)**: change parameters of the pie chart
- **.cget(parameter)**: return the required parameter from the chart

Follow me for more stuff like this: [`Akascape`](https://github.com/Akascape/)
### That's all, hope it will help!

