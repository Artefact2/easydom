easydom
=======

A very simple wrapper around PHP
[DOM](https://secure.php.net/manual/en/book.dom.php). Designed to
reduce the amount of boilerplate code and un-needed verbosity.

~~~
Document (DOMDocument, Appendable)
    ::element(string $name, array $children = []): Element

Element (DOMElement, Appendable, Insertable, Removable, Renderable)
    ::attr(string $name): string
    ::attr(string $name, string $value): Element
    ::hasClass(string $class): bool
    ::addClass(string $class): Element
    ::closestParent(string $name): Element

Node (DOMNode, Appendable, Insertable, Removable, Renderable)

Appendable
    ::append2($content): Appendable
    ::prepend2($content): Appendable
    ::appendCreate(<same as Document::element()>): Element

Insertable
    ::before2(Node $node): void
    ::after2(Node $node): void

Removable
    ::remove(): void

Renderable
    ::renderNode(): string
~~~
