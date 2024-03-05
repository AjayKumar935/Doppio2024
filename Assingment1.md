# Define an XSD schema that validates an XML document containing a list of books with attributes for title, author, and year.


## XML Code
``` xml
<library>
    <book>
        <title>The Atomic Habbits</title>
        <author>James Clear</author>
        <year>2018</year>
    </book>
    <book>
        <title>Rich Dad Poor Dad</title>
        <author>Robert Kiyosaki</author>
        <year>1997</year>
    </book>
    <book>
        <title>The Power of your subconscious mind</title>
        <author>Dr. Joseph Murphy</author>
        <year>1963</year>
    </book>
    
</library>

````

## XSD Code

``` xsd

<xs:schema attributeFormDefault="unqualified" elementFormDefault="qualified" xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <xs:element name="library">
    <xs:complexType>
      <xs:sequence>
        <xs:element name="book" maxOccurs="unbounded" minOccurs="0">
          <xs:complexType>
            <xs:sequence>
              <xs:element type="xs:string" name="title"/>
              <xs:element type="xs:string" name="author"/>
              <xs:element type="xs:short" name="year"/>
            </xs:sequence>
          </xs:complexType>
        </xs:element>
      </xs:sequence>
    </xs:complexType>
  </xs:element>
</xs:schema>

```
