# Diagrams

This template has built-in support for powerful **[mermaid](https://mermaid.js.org/)** diagrams and charts.

The exact definitions of the below examples can be found in the `docs/examples` folder of this template.

## State Diagram

```mermaid
stateDiagram-v2
    [*] --> First
    state First {
        [*] --> true
        true --> [*]
    }

    [*] --> Second
    state Second {
        [*] --> false
        false --> [*]
    }
```

## Sequence Diagram

```mermaid
sequenceDiagram
  Requestor ->> Technical Owner: 1. Some Request
  loop
    Technical Owner -x Requestor: Question 1
    Technical Owner -x Requestor: Question 2
    Technical Owner -x Requestor: ...
  end
  Technical Owner ->> Technical Owner: 2. Approval
  Technical Owner ->> Technical Owner: 3. Update something
  Technical Owner ->> GitHub: 4. Add something
  GitHub ->> Cirrus: 5. Start something
  Cirrus ->> IBM Cloud: 6. Do something
  Technical Owner ->> Requestor: 7. It's all done
  rect rgb(200, 150, 255)
    Technical Owner ->> Requestor: 8. Something else needed
  end
```

## Pie Chart

```mermaid
pie title Votes
  "Yes" : 86
  "No" : 185
  "Maybe" : 25
```

## Flow Chart

```mermaid
flowchart
  A[<b>USER</b>]
  subgraph cirrus ["&nbsp;"]
    AA["<b>APPLICATION (1)</b><br><br>authentication<br>authorization<br>validation<br>..."]
    BB["<b>APPLICATION (2)</b><br><br>authentication<br>authorization<br>validation<br>..."]
    CC["<b>APPLICATION (3)</b><br><br>authentication<br>authorization<br>validation<br>..."]
  end
  subgraph cloud ["&nbsp;"]
    subgraph database3 ["&nbsp;&nbsp;<b>DATABASE (B)</b>&nbsp;&nbsp;"]
      subgraph p3 ["(tables)"]
        direction LR
        h[<b>Table 008</b>]
      end
    end
    subgraph database2 ["&nbsp;&nbsp;<b>DATABASE (B)</b>&nbsp;&nbsp;"]
      subgraph p2 ["(tables)"]
        direction LR
        e[<b>Table 005</b>]
        f[<b>Table 006</b>]
        g[<b>Table 007</b>]
      end
    end
    subgraph database1 ["&nbsp;&nbsp;<b>DATABASE (A)</b>&nbsp;&nbsp;"]
      subgraph p1 ["(tables)"]
        direction LR
        a[<b>Table 001</b>]
        b[<b>Table 002</b>]
        c[<b>Table 003</b>]
        d[<b>Table 004</b>]
      end
    end
  end
  A --->|"https<br>"| AA
  A --->|"https<br>"| BB
  A --->|"https<br>"| CC
  CC -->|"API<br>"| database3
  AA -->|"API<br>"| database1
  BB -->|"API<br>"| database2
```

## XY Chart

```mermaid
xychart
    title "Sales Revenue"
    x-axis [jan, feb, mar, apr, may, jun, jul, aug, sep, oct, nov, dec]
    y-axis "Revenue (in $)" 4000 --> 11000
    bar [5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 7000, 6000]
    line [5000, 6000, 7500, 8200, 9500, 10500, 11000, 10200, 9200, 8500, 7000, 6000]
```

## Gantt Chart

```mermaid
gantt
  title A Gantt Diagram
  dateFormat YYYY-MM-DD
  section Section
      A task          :a1, 2014-01-01, 30d
      Another task    :after a1, 20d
  section Another
      Task in Another :2014-01-12, 12d
      another task    :24d
```

## User Journey

```mermaid
journey
  title My working day
  section Go to work
    Make tea: 5: Me
    Go upstairs: 3: Me
    Do work: 1: Me, Cat
  section Go home
    Go downstairs: 5: Me
    Sit down: 5: Me
```

## Other

Check **[mermaid site](https://mermaid.js.org/)** for many more options.
