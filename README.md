# Regex-ring

[![](https://img.shields.io/github/v/tag/thechampagne/regex?label=version)](https://github.com/thechampagne/regex/releases/latest) [![](https://img.shields.io/github/license/thechampagne/regex)](https://github.com/thechampagne/regex/blob/main/LICENSE)

An easy to use pattern matching for **Ring**.

### Download

```
ringpm install regex
```

### Example

```ring
load "regex.ring"
	
ptrn = "ring"
str = "ring without gems is not a real ring"
re = new Regex(ptrn)
see re.match(str)
# output: ring

for match in re.matchall(str)
    see match
next
/* 
output:
   ring
   ring
*/
```

### License

Regex-ring is released under the [MIT License](https://github.com/thechampagne/regex/blob/main/LICENSE).