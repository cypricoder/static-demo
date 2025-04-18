# Tabs

Tabs let you organize content by context, for example installation instructions for each supported platform.

```tpl
{{</* tabs "id" */>}}
{{%/* tab "MacOS" */%}} # MacOS Content {{%/* /tab */%}}
{{%/* tab "Linux" */%}} # Linux Content {{%/* /tab */%}}
{{%/* tab "Windows" */%}} # Windows Content {{%/* /tab */%}}
{{</* /tabs */>}}
```

## Example

{{< tabs >}}

{{% tab "MacOS" %}}
# MacOS

This is tab **MacOS** content.

Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.
{{% /tab %}}

{{% tab "Linux" %}}
# Linux

This is tab **Linux** content.

Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.
{{% /tab %}}

{{% tab "Windows" %}}
# Windows

This is tab **Windows** content.

Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.
{{% /tab %}}

{{< /tabs >}}

## Example

{{% hint info %}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{% /hint %}}

{{% hint warning %}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{% /hint %}}

{{% hint danger %}}
**Markdown content**  
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
{{% /hint %}}

## Example

```html
{{%/* columns [ratio="1:1"] [class="..."] */%}} <!-- begin columns block -->
# Left Content
Lorem markdownum insigne...

<---> <!-- magic separator, between columns -->

# Mid Content
Lorem markdownum insigne...

<---> <!-- magic separator, between columns -->

# Right Content
Lorem markdownum insigne...
{{%/* /columns */%}}
```

{{% columns %}}
### Left Content
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.

<--->

### Mid Content
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter!

<--->

### Right Content
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.
{{% /columns %}}

## Settings size ratio for columns

```html
{{%/* columns ratio="1:2" */%}} <!-- begin columns block -->

## x1 Column
Lorem markdownum insigne...

<---> <!-- magic separator, between columns -->

## x2 Column
Lorem markdownum insigne...

{{%/* /columns */%}}
```

{{% columns ratio="1:2" %}}
### x1 Column
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.

<--->

### x2 Column
Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter!

Lorem markdownum insigne. Olympo signis Delphis! Retexi Nereius nova develat
stringit, frustra Saturnius uteroque inter! Oculis non ritibus Telethusa
protulit, sed sed aere valvis inhaesuro Pallas animam: qui _quid_, ignes.
Miseratus fonte Ditis conubia.

{{% /columns %}}

## Example

```tpl
{{</* button relref="/" [class="..."] */>}}Get Home{{</* /button */>}}
{{</* button href="https://github.com/alex-shpak/hugo-book" */>}}Contribute{{</* /button */>}}
```

{{<button relref="/">}}Get Home{{</button>}}
{{<button href="https://github.com/alex-shpak/hugo-book">}}Contribute{{</button>}}

## Example


{{% columns %}}

```tpl
{{</* mermaid [class="..."] >}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{< /mermaid */>}}
```

<--->

{{<mermaid>}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{</mermaid>}}

{{% /columns %}}
