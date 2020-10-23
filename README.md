#  Markdown stuff
## Level 2 heading blah **blah**

### To-do list
- Learn git
- practice BASH
- update CV
- write programmes

Link to [the course](https://github.com/seankross/the-unix-workbench) on unix and bash

## My fibonacci function

```
function fib {

local l0=1
local l1=0
if [[ $1 -eq 1 ]]
  then echo 0
elif [[ $1 -eq 2 ]]
  then echo "0 1"
else
  local arr=($l1 $l0)
  for((index=3;index<=$1;index++))
  do
    let l=l1+l0 
    let l1=l0
    let l0=l
    arr+=($l)
  done
  echo ${arr[*]}
fi
}
```
