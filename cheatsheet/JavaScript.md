Resource
Online

    Official Website

Download

    JavaScript Cheat Sheet [.pdf]
    JavaScript Quick Reference Card [.pdf]
    JavaScript and Browser Objects Quick Reference [.pdf]
    JavaScript in one page

Related

```js
AJAX
CSS
HTML DOM
GWT
HTML
jQuery
MooTools
Node.js
Prototype
XHTML
```

Basic Objects
Array Properties

    constructor
    length
    prototype

Array Methods

```js
concat()
indexOf()
join()
lastIndexOf()
pop()
push()
reverse()
shift()
slice()
sort()
splice()
toString()
unshift()
valueOf()
```

Boolean Properties

    constructor
    prototype

Boolean Methods

    toString()
    valueOf()

Math Properties

    E
    LN2
    LN10
    LOG2E
    LOG10E
    PI
    SQRT1_2
    SQRT2

Math Methods

    abs(x)
    acos(x)
    asin(x)
    atan(x)
    atan2(y,x)
    ceil(x)
    cos(x)
    exp(x)
    floor(x)
    log(x)
    max(x,y,z,...,n)
    min(x,y,z,...,n)
    pow(x,y)
    random()
    round(x)
    sin(x)
    sqrt(x)
    tan(x)

Number Properties

    constructor
    MAX_VALUE
    MIN_VALUE
    NEGATIVE_INFINITY
    POSITIVE_INFINITY
    prototype

Number Methods

    toExponential(x)
    toFixed(x)
    toPrecision(x)
    toString()
    valueOf()

String Properties

    constructor
    length
    prototype

String Methods

    charAt()
    charCodeAt()
    concat()
    fromCharCode()
    indexOf()
    lastIndexOf()
    match()
    replace()
    search()
    slice()
    split()
    substr()
    substring()
    toLowerCase()
    toUpperCase()
    valueOf()

String HTML Wrapper Methods

    anchor()
    big()
    blink()
    bold()
    fixed()
    fontcolor()
    fontsize()
    italics()
    link()
    small()
    strike()
    sub()
    sup()

Global Properties

    Infinity
    NaN
    undefined

Global Methods

    decodeURI()
    decodeURIComponent()
    encodeURI()
    encodeURIComponent()
    escape()
    eval()
    isFinite()
    isNaN()
    Number()
    parseFloat()
    parseInt()
    String()
    unescape()

Date Object
Date Properties

    constructor
    prototype

Date Methods

    getDate()
    getDay()
    getFullYear()
    getHours()
    getMilliseconds()
    getMinutes()
    getMonth()
    getSeconds()
    getTime()
    getTimezoneOffset()
    getUTCDate()
    getUTCDay()
    getUTCFullYear()
    getUTCHours()
    getUTCMilliseconds()
    getUTCMinutes()
    getUTCMonth()
    getUTCSeconds()
    parse()
    setDate()
    setFullYear()
    setHours()
    setMilliseconds()
    setMinutes()
    setMonth()
    setSeconds()
    setTime()
    setUTCDate()
    setUTCFullYear()
    setUTCHours()
    setUTCMilliseconds()
    setUTCMinutes()
    setUTCMonth()
    setUTCSeconds()
    toDateString()
    toISOString()
    toJSON()
    toLocaleDateString()
    toLocaleTimeString()
    toLocaleString()
    toString()
    toTimeString()
    toUTCString()
    UTC()
    valueOf()

Browser
Window Properties

```js
closed
defaultStatus
document
frames
history
innerHeight
innerWidth
length
location
name
navigator
opener
outerHeight
outerWidth
pageXOffset
pageYOffset
parent
screen
screenLeft
screenTop
screenX
screenY
self
status
top
```

Window Methods

    alert()
    blur()
    clearInterval()
    clearTimeout()
    close()
    confirm()
    focus()
    moveBy()
    moveTo()
    open()
    print()
    prompt()
    resizeBy()
    resizeTo()
    scrollBy()
    scrollTo()
    setInterval()
    setTimeout()

Navigator Properties

    appCodeName
    appName
    appVersion
    cookieEnabled
    platform
    userAgent

Navigator Methods

    javaEnabled()
    registerContentHandler()
    registerProtocolHandler()

Screen Properties

    availHeight
    availWidth
    colorDepth
    height
    pixelDepth
    width

History Properties

    length

History Methods

    back()
    forward()
    go()

Location Properties

    hash
    host
    hostname
    href
    pathname
    port
    protocol
    search

Location Methods

    assign()
    reload()
    replace()

DOM Events
Mouse Events

    click
    dblclick
    mousedown
    mousemove
    mouseover
    mouseout
    mouseup

Keyboard Events

    keydown
    keypress
    keyup

Frame Events

    abort
    error
    load
    resize
    scroll
    unload

Form Events

    blur
    change
    focus
    reset
    select
    onsubmit

Event Object Constant

    AT_TARGET
    BUBBLING_PHASE
    CAPTURING_PHASE

Event Object Properties

    bubbles
    cancelable
    currentTarget
    eventPhase
    target
    timeStamp
    type

Event Object Methods

    initEvent()
    preventDefault()
    stopPropagation()

EventTarget Object

    addEventListener()
    dispatchEvent()
    removeEventListener()

EventListener Object

    handleEvent()

MouseEvent/KeyboardEvent Object

    altKey
    button
    clientX
    clientY
    ctrlKey
    keyIdentifier
    keyLocation
    metaKey
    relatedTarget
    screenX
    screenY
    shiftKey

MouseEvent/KeyboardEvent Methods

    initMouseEvent()
    initKeyboardEvent()

DOM Node
Node Properties

    attributes
    baseURI
    childNodes
    firstChild
    lastChild
    localName
    namespaceURI
    nextSibling
    nodeName
    nodeType
    nodeValue
    ownerDocument
    parentNode
    prefix
    previousSibling
    textContent

Node Methods

    appendChild()
    cloneNode()
    compareDocumentPosition()
    getFeature(feature,version)
    getUserData(key)
    hasAttributes()
    hasChildNodes()
    insertBefore()
    isDefaultNamespace()
    isEqualNode()
    isSameNode()
    isSupported()
    lookupNamespaceURI()
    lookupPrefix()
    normalize()
    removeChild()
    replaceChild()
    setUserData(key,data,handler)

Node Types

    Element1
    Attr2
    Text3
    CDATASection4
    EntityReference5
    Entity6
    ProcessingInstruction7
    Comment8
    Document9
    DocumentType10
    DocumentFragment11
    Notation12

nodeName Returns

    Element
    element name
    Attr
    attribute name
    Text
    #text
    CDATASection
    #cdata-section
    EntityReference
    entity reference name
    Entity
    entity name
    ProcessingInstruction
    target
    Comment
    #comment
    Document
    #document
    DocumentType
    doctype name
    DocumentFragment
    #document fragment
    Notation
    notation name

nodeValue Returns

    Element
    null
    Attr
    attribute value
    Text
    content of node
    CDATASection
    content of node
    EntityReference
    null
    Entity
    null
    ProcessingInstruction
    content of node
    Comment
    comment text
    Document
    null
    DocumentType
    null
    DocumentFragment
    null
    Notation
    null

RegExp
Modifiers

    i
    Perform case-insensitive matching
    g
    Perform a global match (find all matches rather than stopping after the first match)
    m
    Perform multiline matching

Brackets

    [abc]
    Find any character between the brackets
    [^abc]
    Find any character not between the brackets
    [0-9]
    Find any digit from 0 to 9
    [A-Z]
    Find any character from uppercase A to uppercase Z
    [a-z]
    Find any character from lowercase a to lowercase z
    [A-z]
    Find any character from uppercase A to lowercase z
    [adgk]
    Find any character in the given set
    [^adgk]
    Find any character outside the given set
    (red|blue|green)
    Find any of the alternatives specified

Metacharacters

    .
    Find a single character, except newline or line terminator
    \w
    Find a word character
    \W
    Find a non-word character
    \d
    Find a digit
    \D
    Find a non-digit character
    \s
    Find a whitespace character
    \S
    Find a non-whitespace character
    \b
    Find a match at the beginning/end of a word
    \B
    Find a match not at the beginning/end of a word
    \0
    Find a NUL character
    \n
    Find a new line character
    \f
    Find a form feed character
    \r
    Find a carriage return character
    \t
    Find a tab character
    \v
    Find a vertical tab character
    \xxx
    Find the character specified by an octal number xxx
    \xdd
    Find the character specified by a hexadecimal number dd
    \uxxxx
    Find the Unicode character specified by a hexadecimal number xxxx

Quantifiers

    n+
    Matches any string that contains at least one n
    n*
    Matches any string that contains zero or more occurrences of n
    n?
    Matches any string that contains zero or one occurrences of n
    n{X}
    Matches any string that contains a sequence of X n's
    n{X,Y}
    Matches any string that contains a sequence of X to Y n's
    n{X,}
    Matches any string that contains a sequence of at least X n's
    n$
    Matches any string with n at the end of it
    ^n
    Matches any string with n at the beginning of it
    ?=n
    Matches any string that is followed by a specific string n
    ?!n
    Matches any string that is not followed by a specific string n

RegExp Properties

    global
    ignoreCase
    lastIndex
    multiline
    source

RegExp Methods

    exec()
    test()