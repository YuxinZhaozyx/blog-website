---
title: "Shortcodes"
date: 2019-09-21T13:58:33+08:00
draft: false
tags: ["shortcode"]
categories: ["example"]

toc: true
autoCollapseToc: true

comment: true

mathjax: true
mathjaxEnableSingleDollar: false
mathjaxEnableAutoNumber: false

reward: false

hiddenFromHomePage: true

flowchartDiagrams:
  enable: false
  options: ""

sequenceDiagrams: 
  enable: false
  options: ""
---



# Admonition

```markdown
{{%/* admonition note "I'm title!" false */%}}
A example with title

{{%/* admonition type="note" title="note" details="true" */%}}
This is a example
{{%/* /admonition */%}}

{{%/* admonition example */%}}
Without title.
{{%/* /admonition */%}}

{{%/* /admonition */%}}
```

{{% admonition note "I'm title!" false %}}
A example with title

{{% admonition type="note" title="note" details="true" %}}
This is a example
{{% /admonition %}}

{{% admonition example %}}
Without title.
{{% /admonition %}}

{{% /admonition %}}

<!--more-->

---

```markdown
{{%/* admonition abstract abstract */%}}
biu biu biu.
{{%/* /admonition */%}}
```

{{% admonition abstract abstract %}}
biu biu biu.
{{% /admonition %}}

```markdown
{{%/* type="abstract" title="abstract" details="true" */%}}
biu biu biu.
{{%/* /admonition */%}}
```

{{% admonition type="abstract" title="abstract" details="true" %}}
biu biu biu.
{{% /admonition %}}

---

## More Admonitions

{{% admonition info "info" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition tip "tip" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition success "success" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition question "question" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition warning "warning" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition failure "failure" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition danger "danger" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition bug "bug" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition example "example" %}}
biu biu biu.
{{% /admonition %}}

{{% admonition quote "quote" %}}
biu biu biu.
{{% /admonition %}}

---

# Music 163

## Params
- `id`
  - required param
  - you can extract from music url
  - url format http://music.163.com/#/song?id=28196554

- Fiddle `auto`
  - optional param
  - default value 0
  - you can overwrite it with 1

## Examples

- Simple

```
{{%/* music 28196554 */%}}
{{%/* music 28196554  1 */%}}
```

- Named Params

```
{{%/* music id="28196554" */%}}
{{%/* music id="28196554" auto="1" */%}}
```

- Example

```
{{%/* music 28196554 */%}}
```

{{% music 28196554 %}}

---

# Bilibili video

## Params

+ `av`
  + id of the bilibili video
  + you can extract from bilibili video url
  + url format https://www.bilibili.com/video/av65010879
+ `page`
  + which page to display
  + option param
  + default value 1

## Example

+ Simple

```markdown
{{%/* bilibili 65010879 */%}}
{{%/* bilibili 65010879 1 */%}}
```

+ Named Params

```markdown
{{%/* bilibili av="65010879" */%}}
{{%/* bilibili av="65010879" page="1" */%}}
```

+ Example

```markdown
{{%/* bilibili 65010879 */%}}
```

{{% bilibili 65010879 %}}



