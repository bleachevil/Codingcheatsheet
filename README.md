# Codingcheatsheet

## Markdown Syntax

#### Table

| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |


#### Fenced Code Block (Copy code)

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
```python
print("hello world")
```

#### Footnote
Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.


#### Heading ID ???

### My Great Heading {#custom-id}

#### Space

i love you<br />
you love me

#### Definition List

term
: definition


#### Strikethrough

~~The world is flat.~~

#### Take List

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media


#### Emoji

That is so funny! :joy:

#### Textsize

## Codingcheatsheet
### Codingcheatsheet


#### Bold

**my name is Jeff, i am business planning manager**


#### Highlight ??

I need to highlight these ==very important words==.


####  line
<hr />

#### Italic

*I live downtown mississagua*

#### Picture

![](https://github.com/bleachevil/Codingcheatsheet/blob/main/download.jpg?raw=true)


#### Subscript

H~2~O

#### Superscript

X^2^


<hr />
https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax

## Git

```git
git add
```
```git
git commit -m ""
```
```git
git push origin main
```

# Python

## control C 
to stop

## day and time only
```
YEAR        = datetime.date.today().year
MONTH       = datetime.date.today().month
DATE        = datetime.date.today().day
HOUR        = datetime.datetime.now().hour
MINUTE      = datetime.datetime.now().minute
SECONDS     = datetime.datetime.now().second
```
print(YEAR, MONTH, DATE, HOUR, MINUTE, SECONDS)

## add variable with text
```
print(f"text {variable}")
```

## equal sign
```
one = sign is variable assignment 
two == is the confirmatin of the equal
!= mean is not equal
```

## Boolean (Computer logic operation)
```
age == 21 True
age > 21 False
age <= 21 True
age != 21 False
```

## list vs Tuper
a [1,2,3,]   access the list by index
b = [ (John,1), (Allen,2)]

## calculation

** = ^
% = /

## reverse list
a[:: -1]

## jump 2
if x / 2 ==0
list[0::2]

## while
```
i = 1
while i < 6:
  print(i)
  i += 1
```
**stop at 5**
```
i = 1
while i < 6:
  print(i)
  if i == 3:
    break
  i += 1  #same i = i+1
```
**stop at 3**

```
i = 0
while i < 6:
  i += 1
  if i == 3:
    continue
  print(i)
```
**start with 3 and finishe until 5**

## arrart slicing
a[-3:] last 3
a[:3] last 3

a[:-3] first 2

a[1:3] the 1 is including and 3 is excluding

a[:: 2] every other element the arrary.

a[:: -1] reverse array


## list
add two list 
[var+var]


## queue vs stack
queue = FIFO
Stack = LIFO
collection model

a.append() add item in the list
a.pop() stack impliementation  remove the list
a.pop(position) position = index 1,2,3,4 remove the one the in the index
append + pop(0) = queue
append + pop = stack

a.index('position')
a.insert(index, item) example a.insert(1,'no')
a.remove('no') only remove first one add

a_np = a.array(
np.ramdom.sample(1)

## tuple
tuple(enumerate(list))
dict(enumerate(list))

##  json is dictionary
key value pair of

list.keys()   = the keys
list.values() = the values

Dict[4] = value 
del Dict[4]




## function
input to output

## import csv
rows = []

file = open('file.csv')
csvreader = csv.reader(file)
header = next(csvreader)
print(header)
for row in csvreader:
    rows.append(row)

## split
list = []

option1 = res1, res2 = map(list, zip(*list))
option2 = res1 = [i[1] for i in list], 
res2 = [i[0] for i in list]


## search in the list
Greatest = max(res2)
for Great in rows:
    if Greatest in Great:
        element_in_lists = True
        
## day
from datetime import date, timedelta
import datetime
 
today = date.today()
td = timedelta(1001)
open_day = today - td
close_day = today - timedelta(1) 
openeday = open_day.strftime("%Y-%m-%d")
closeday = close_day.strftime("%Y-%m-%d")

## multiindex columns
data = alpaca.get_bars('AGG', TimeFrame.Day, start_date, end_date, adjustment='raw').df
data.drop(columns=['trade_count','vwap'], inplace=True)
name = 'AGG'
#data.index=data.index.date
col = pd.MultiIndex.from_product([[name],data.columns])
col
data.columns = col
data

data2 = alpaca.get_bars('SPY', TimeFrame.Day, start_date, end_date, adjustment='raw').df
data2.drop(columns=['trade_count','vwap'], inplace=True)
name2 = 'SPY'
#data2.index=data2.index.date
col2 = pd.MultiIndex.from_product([[name2],data2.columns])
col2
data2.columns = col2
data2
df_stock_data = data.merge(data2, how="inner", left_index=True, right_index=True)
df_stock_data
# Display sample data
df_stock_data.head()

## data vision
https://hvplot.holoviz.org/reference/pandas/scatter.html#pandas-gallery-scatter

## groupby
df.groupby('Company Name')['Amount'].agg(['sum','count'])
df.groupby('Company Name').agg({'Amount': ['sum','count']}


### formula

x7 = (x5 – 1)(6/4) + 1

