# chart-notes-data
This repo stores note data of Arcaea chart.

## For each json:

Data are stored in big json object, with `songid` as key and an array for note data as value.

If the length of array value is 3, then:

- `arr[0]` is for PST difficulty
- `arr[1]` is for PRS difficulty
- `arr[2]` is for FTR difficulty

If the length of array value is 4, beside for those mentioned before, the 4th element of array `arr[3]` is for BYD difficulty.

**Note:** The length of array must be at least 3. So for april fool songs that has no PST and PRS difficulties, the value is -1 for them.

```json
{
  "ignotusafterburn": [-1, -1, 1028]
}
```
