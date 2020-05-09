# word_square_bracket_bibliography
word square bracket bibliography ISO690Nmerical ISO690 Numerical 

## why
In Word 2016, the ISO 690 Numeric style in the bibliography is shown as standard in parentheses __(number)__, and as I needed it to appear in square brackets __[number]__.

W Wordzie 2016 styl ISO690 Numeryczny w bibliografii pokazuje się standarowo w nawiasach zwykłych __(numer)__, a jak potrzebowałem aby pojawiał sie w nawiasach kwadratowych __[numer]__.

## files to modify


`C:\Users\<user>\AppData\Roaming\Microsoft\Bibliography\Style\ISO690Nmerical.XSL`
for \<__selected user__\> -> ***so it's needed for all users***

`C:\Program Files\Microsoft Office\root\Office16\Bibliography\Style\ISO690Nmerical.XSL`
=> as I understand only for **NEW** word user
 
## modification to do

```xsl
<xsl:template name="templ_prop_OpenBracket" >
<!--    <xsl:param name="LCID" />
    <xsl:variable name="_LCID">
      <xsl:call-template name="localLCID">
        <xsl:with-param name="LCID" select="$LCID"/>
      </xsl:call-template>
    </xsl:variable>
    <xsl:value-of select="/*/b:Locals/b:Local[@LCID=$_LCID]/b:General/b:OpenBracket"/>-->
    <xsl:text>[</xsl:text>
  </xsl:template>

  <xsl:template name="templ_prop_CloseBracket" >
<!--    <xsl:param name="LCID" />
    <xsl:variable name="_LCID">
      <xsl:call-template name="localLCID">
        <xsl:with-param name="LCID" select="$LCID"/>
      </xsl:call-template>
    </xsl:variable>
    <xsl:value-of select="/*/b:Locals/b:Local[@LCID=$_LCID]/b:General/b:CloseBracket"/> -->
   <xsl:text>]</xsl:text>
  </xsl:template>
```

## final file:
[file do download \<ISO690Nmerical.XSL\>](../blob/master/ISO690Nmerical.XSL)
