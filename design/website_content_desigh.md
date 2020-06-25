# The content design

## Introduction

This fils introduces the content of the website and the relationship between website and the repo *community*.

## What to sychronize

In the website, there are the followin menues:

- Homepage which you can click the logo in the up left to reach

- Download where you can download software

- Documentation which includes quich starts and the main doc

- Community which includes

    - Contribution

    - Who we are

    - Communication, which includes Mail list and Slack. 

- Newsroom which includes 
    
    - News

    - Events

    - Blog

The content of governance will be added into the page *Community/Who we are*.

## The required format of the files

In case there is anything to synchronize the content to website, the folder should be designed as below:

- Folder structure of *content* in this repo.

```
|-- en
    |-- openLooKeng Governance
        |-- _index.md
    |-- Project Management Committee
        |-- _index.md
    |-- Committers
        |-- _index.md
    |-- QA
        |-- _index.md
    |-- User Group
        |-- _index.md
    |-- Secretary
        |-- _index.md
|-- zh
// which are kept the same as the folder en.

```

Take the example of *openLooKeng Governance*. It is a flolder and will be in the left menu. When it is clicked, the content of _index.md under it is displayed.

The formart of _index.md is markdown but it need follow the following special format.

- The head of the file

```
+++
bookCollapseSection = "true"
weight = 2

# Introduction

+++

For details please refer to [website design](https://gitee.com/openlookeng/website/tree/master/design).

```

## How to publish the content to website?

1 Authors update the content and get merged to the branch **master**

1 The update under the folder *content* is synchronized to the repo website in real time.

1 In the website repo, a new tag will be added and then it will be committed to the brand *stabel* manually. 

1 Finally the updated website is built and published.

----End of the file---
