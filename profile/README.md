# Practal — Practical Logic: A Bicyle for Your Mathematical Mind

For background information of *Practal* and its vision, please also check out [practal.com](https://practal.com).

Currently, only [me](https://github.com/phlegmaticprogrammer) is working on *Practal*. Hopefully that will change in 2023! 

Before that can happen, I first need to firmly establish the roots of the project. Early research prototypes have been implemented in [Swift](https://docs.swift.org/swift-book/), but in order to make Practal as widely available as possible, all development has been shifted to [TypeScript](https://www.typescriptlang.org).

Much is planned for 2023, illustrated in the following graphic:

<img width="100%" src="profile/products.png">

The graphic shows several planned, highly interdependent products: two web apps, and six supporting open-source TypeScript packages.
Let's see what each of these products is about in a bit more detail. 

## *Practal*

The *Practal* web app is the long-term and ultimate goal. Its purpose is to be a [bicycle for your mathematical mind](https://practal.com). 

If that sounds too vague for you, imagine instead something of a fusion of interactive theorem proving systems like [Isabelle](https://isabelle.in.tum.de), with systems like [SageMath](https://www.sagemath.org), word processing technologies inspired by LaTeX, [Markdown](https://daringfireball.net/projects/markdown/) and [Obsidian](https://obsidian.md), and AI capabilities inspired by systems such as [ChatGPT](https://openai.com/blog/chatgpt).

While there is no way that Practal can be fully realized in 2023, a first version is planned for not later than September 2023. 

## *Practal Core*

*Practal Core* will be an open source TypeScript package implementing core concepts of Practal such as [*Abstraction Algebra* and *Abstraction Logic*](https://obua.com/publications/philosophy-of-abstraction-logic/2/). Besides functioning as a library which you can import into your own projects, it will also provide command line utilities and a terminal REPL. Practal Core enables you to make use of all artefacts created with the Practal app wherever and however you want to. 

Practal Core is released in tandem with releases of Practal.

## *Grammar.design*

The *Grammar.design* web app has also been a vision of mine for quite some time, and it now is within reach. Its realization is the goal of the first few months of 
2023. Its purpose is to make designing and testing [*Pyramid Grammars*](https://obua.com/publications/local-lexing/1/) simple.  

At the same time, it represents an important step towards Practal. Many of the technologies used for Grammar.design will also be used for Practal. There are two reasons for this:
1. An important part of using logic in practice is how you denote concepts via syntax. Pyramid grammars allow you to specify syntax in a composable and collaborative fashion.
1. From a conceptual point of view, Grammar.design is all about working with a formal model, in this case pyramid grammars. From that point of view, Grammar.design is actually a special case of Practal! If you accept this point of view, then you will also start to understand the full potential of Practal.

A first version of Grammar.design is scheduled for February 2023.

## *Pyramids*

*Pyramids* is an open-source TypeScript package for working and parsing with pyramid grammars, and contains the [technology](https://obua.com/publications/local-lexing/1/) 
on which Grammar.design is based. It will enable you to make use of all artefacts created via the Grammar.design app. 

A first version of Pyramids is scheduled for January 2023.

## *Teace* and *Pyramidion*

These are open-source TypeScript packages in the making to implement editing facilities for both Grammar.design and Practal. 

The purpose of *Teace* is to implement a flexible approach to editing based on HTML's [`contenteditable`](https://developer.mozilla.org/en-US/docs/Web/HTML/Global_attributes/contenteditable). It is roughly inspired by
[The Elm Architecture](https://guide.elm-lang.org/architecture/), and infuses ideas from [Lexical](https://lexical.dev), [ProseMirror](https://prosemirror.net) and [Slate.js](https://www.slatejs.org).

*Pyramidion* is a plugin for Teace that makes it possible to edit text based on the structure prescribed by pyramid grammars. 

A first release of both packages is expected together with the first release of Grammar.design.

## *Things* and *InstaTest*

These two open-source TypeScript packages provide the infrastructure for *hardened functional programming and testing in TypeScript*. 

The problem with JavaScript, and consequentially also with TypeScript, is that by default very little runtime guarantees are provided. For example, methods can be removed and added to objects by anyone, making it hard for an API to guarantee any invariants. The *Things* package introduces data structures and tools to combat this problem, mainly through *freezing* and *purely functional data structures*. Additionally, the *InstaTest* package provides a simple and lightweight testing framework.

Both [Things](https://github.com/practal/things) and [InstaTest](https://github.com/practal/instatest) are available, but still highly experimental and subject to rapid and extreme change.

## Funding

The two web apps will be published under a Freemium business model based on subscriptions. The hope is that this enables sustained development and availability of resources, such that Practal and Grammar.design can eventually become everyday infrastructure. 

To ensure that this infrastructure can be used without worrying about lock-in, core components of Practal and Grammar.design are published as open-source projects. Please consider donating to them. This will soon be possible via GitHub Sponsors, and help a lot!





