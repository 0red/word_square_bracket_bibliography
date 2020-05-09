# word_square_bracket_bibliography
word square bracket bibliography ISO690Nmerical ISO690 Numerical 

## why
In Word 2016  ISO690 Numerical citation reference appear as __(number)__ but I need __[number]__

## files to modify


C:\Users\<user>\AppData\Roaming\Microsoft\Bibliography\Style\ISO690Nmerical.XSL
for <user> --> so it's needed for all users

C:\Program Files\Microsoft Office\root\Office16\Bibliography\Style\ISO690Nmerical.XSL
as I understand only for NEW created user
 
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
  `
