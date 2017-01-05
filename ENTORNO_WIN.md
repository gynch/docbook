# Preparación del entorno para Windows

## Configuración del editor ATOM

En primer lugar configuraré el editor ATOM para trabajar cómodamente con documentos XML Docbook.

Para ello he añadido los snippets siguientes a snippets.cson
Estos snippets provienen prácticamente en su totalidad del  [repositorio de pbokoc en github](https://github.com/pbokoc/atom-docbook-snippets) 

```
# Your snippets
#
# Atom snippets allow you to enter a simple prefix in the editor and hit tab to
# expand the prefix into a larger code block with templated values.
#
# You can create a new snippet in this file by typing "snip" and then hitting
# tab.
#
# An example CoffeeScript snippet to expand log to console.log:
#
# '.source.coffee':
#   'Console log':
#     'prefix': 'log'
#     'body': 'console.log $1'
#
# Each scope (e.g. '.source.coffee' above) can only be declared once.
#
# This file uses CoffeeScript Object Notation (CSON).
# If you are unfamiliar with CSON, you can read more about it in the
# Atom Flight Manual:
# http://flight-manual.atom.io/using-atom/sections/basic-customization/#_cson
	'.xml':
		'abbrev':
			'prefix': 'abbrev'
			'body': """
			<abbrev>${1}</abbrev>
			"""
		'abstract':
			'prefix': 'abstract'
			'body': """
			<abstract>
					${1}
			</abstract>
			"""
		'accel':
			'prefix': 'accel'
			'body': """
			<accel>${1}</accel>
			"""
		'ackno':
			'prefix': 'ackno'
			'body': """
			<ackno>
					${1}
			</ackno>
			"""
		'acronym':
			'prefix': 'acronym'
			'body': """
			<acronym>${1}</acronym>
			"""
		'action':
			'prefix': 'action'
			'body': """
			<action>${1}</action>
			"""
		'address':
			'prefix': 'address'
			'body': """
			<address>
				${1}
			</address>
			"""
		'affiliation':
			'prefix': 'affiliation'
			'body': """
			<affiliation>
				${1}
			</affiliation>
			"""
		'alt':
			'prefix': 'alt'
			'body': """
			<alt>${1}</alt>
			"""
		'anchor':
			'prefix': 'anchor'
			'body': """
			<anchor id="${1}" />
			"""
		'answer':
			'prefix': 'answer'
			'body': """
			<answer>
				${1}
			</answer>
			"""
		'appendix':
			'prefix': 'appendix'
			'body': """
			<appendix id="${1}">
				${2}
			</appendix>
			"""
		'appendixinfo':
			'prefix': 'appendixinfo'
			'body': """
			<appendixinfo>
				${1}
			</appendixinfo>
			"""
		'application':
			'prefix': 'application'
			'body': """
			<application>${1}</application>
			"""
		'area':
			'prefix': 'area'
			'body': """
			<area id="${1}" coords="${2}" />
			"""
		'areaset':
			'prefix': 'areaset'
			'body': """
			<areaset id="${1}">
				${2}
			</areaset>
			"""
		'areaspec':
			'prefix': 'areaspec'
			'body': """
			<areaspec units="${1}">
				${2}
			</areaspec>
			"""
		'arg':
			'prefix': 'arg'
			'body': """
			<arg>${1}</arg>
			"""
		'article':
			'prefix': 'article'
			'body': """
			<article id="${1}">
				${2}
			</article>
			"""
		'articleinfo':
			'prefix': 'articleinfo'
			'body': """
			<articleinfo>
				${1}
			</articleinfo>
			"""
		'artpagenums':
			'prefix': 'artpagenums'
			'body': """
			<artpagenums>${1}</artpagenums>
			"""
		'attribution':
			'prefix': 'attribution'
			'body': """
			<attribution>${1}</attribution>
			"""
		'audiodata':
			'prefix': 'audiodata'
			'body': """
			<audiodata fileref="${1}" />
			"""
		'audioobject':
			'prefix': 'audioobject'
			'body': """
			<audioobject>
				${1}
			</audioobject>
			"""
		'author':
			'prefix': 'author'
			'body': """
			<author>
				${1}
			</author>
			"""
		'authorblurb':
			'prefix': 'authorblurb'
			'body': """
			<authorblurb>
				${1}
			</authorblurb>
			"""
		'authorgroup':
			'prefix': 'authorgroup'
			'body': """
			<authorgroup>
				${1}
			</authorgroup>
			"""
		'authorinitials':
			'prefix': 'authorinitials'
			'body': """
			<authorinitials>${1}</authorinitials>
			"""
		'beginpage':
			'prefix': 'beginpage'
			'body': """
			<beginpage pagenum="${1}" />
			"""
		'bibliocoverage':
			'prefix': 'bibliocoverage'
			'body': """
			<bibliocoverage>
				${1}
			</bibliocoverage>
			"""
		'bibliodiv':
			'prefix': 'bibliodiv'
			'body': """
			<bibliodiv>
				${1}
			</bibliodiv>
			"""
		'biblioentry':
			'prefix': 'biblioentry'
			'body': """
			<biblioentry>
				${1}
			</biblioentry>
			"""
		'bibliography':
			'prefix': 'bibliography'
			'body': """
			<bibliography id="${1}">
				${2}
			</bibliography>
			"""
		'bibliographyinfo':
			'prefix': 'bibliographyinfo'
			'body': """
			<bibliographyinfo>
				${1}
			</bibliographyinfo>
			"""
		'biblioid':
			'prefix': 'biblioid'
			'body': """
			<biblioid class="${1:isbn}">${2}</biblioid>
			"""
		'bibliolist':
			'prefix': 'bibliolist'
			'body': """
			<bibliolist>
				${1}
			</bibliolist>
			"""
		'bibliomisc':
			'prefix': 'bibliomisc'
			'body': """
			<bibliomisc>
				${1}
			</bibliomisc>
			"""
		'bibliomixed':
			'prefix': 'bibliomixed'
			'body': """
			<bibliomixed>
				${1}
			</bibliomixed>
			"""
		'bibliomset':
			'prefix': 'bibliomset'
			'body': """
			<bibliomset relation="${1}">
				${2}
			</bibliomset>
			"""
		'biblioref':
			'prefix': 'biblioref'
			'body': """
			<biblioref linkend="${1}" />
			"""
		'bibliorelation':
			'prefix': 'bibliorelation'
			'body': """
			<bibliorelation type="${1}" class="${2}">${3}</bibliorelation>
			"""
		'biblioset':
			'prefix': 'biblioset'
			'body': """
			<biblioset relation="${1}">
				${2}
			</biblioset>
			"""
		'bibliosource':
			'prefix': 'bibliosource'
			'body': """
			<bibliosource class="${1:isbn}">${2}</bibliosource>
			"""
		'blockinfo':
			'prefix': 'blockinfo'
			'body': """
			<blockinfo>
				${1}
			</blockinfo>
			"""
		'blockquote':
			'prefix': 'blockquote'
			'body': """
			<blockquote>
				${1}
			</blockquote>
			"""
		'book':
			'prefix': 'book'
			'body': """
			<book id="${1}">
				${2}
			</book>
			"""
		'bookinfo':
			'prefix': 'bookinfo'
			'body': """
			<bookinfo>
				${1}
			</bookinfo>
			"""
		'bridgehead':
			'prefix': 'bridgehead'
			'body': """
			<bridgehead renderas="${1:sect3}">${2}</bridgehead>
			"""
		'callout':
			'prefix': 'callout'
			'body': """
			<callout arearefs="${1}">
				${2}
			</callout>
			"""
		'calloutlist':
			'prefix': 'calloutlist'
			'body': """
			<calloutlist>
				${1}
			</calloutlist>
			"""
		'caption':
			'prefix': 'caption'
			'body': """
			<caption>
				${1}
			</caption>
			"""
		'caution':
			'prefix': 'caution'
			'body': """
			<caution>
				${1}
			</caution>
			"""
		'chapter':
			'prefix': 'chapter'
			'body': """
			<chapter id="${1}">
				${2}
			</chapter>
			"""
		'chapterinfo':
			'prefix': 'chapterinfo'
			'body': """
			<chapterinfo>
				${1}
			</chapterinfo>
			"""
		'citation':
			'prefix': 'citation'
			'body': """
			<citation>${1}</citation>
			"""
		'citebiblioid':
			'prefix': 'citebiblioid'
			'body': """
			<citebiblioid class="${1:isbn}">${2}</citebiblioid>
			"""
		'citerefentry':
			'prefix': 'citerefentry'
			'body': """
			<citerefentry>${1}</citerefentry>
			"""
		'citetitle':
			'prefix': 'citetitle'
			'body': """
			<citetitle pubwork="${1:book}">${2}</citetitle>
			"""
		'city':
			'prefix': 'city'
			'body': """
			<city>${1}</city>
			"""
		'classname':
			'prefix': 'classname'
			'body': """
			<classname>${1}</classname>
			"""
		'classsynopsis':
			'prefix': 'classsynopsis'
			'body': """
			<classsynopsis class="${1}" language="${2}">
				${3}
			</classsynopsis>
			"""
		'classsynopsisinfo':
			'prefix': 'classsynopsisinfo'
			'body': """
			<classsynopsisinfo>
				${1}
			</classsynopsisinfo>
			"""
		'cmdsynopsis':
			'prefix': 'cmdsynopsis'
			'body': """
			<cmdsynopsis>
				${1}
			</cmdsynopsis>
			"""
		'co':
			'prefix': 'co'
			'body': """
			<co label="${1}" linkends="${2}" />
			"""
		'code':
			'prefix': 'code'
			'body': """
			<code language="${1}">${2}</code>
			"""
		'col':
			'prefix': 'col'
			'body': """
			<col>
				${1}
			</col>
			"""
		'colgroup':
			'prefix': 'colgroup'
			'body': """
			<colgroup>
				${1}
			</colgroup>
			"""
		'collab':
			'prefix': 'collab'
			'body': """
			<collab>
				${1}
			</collab>
			"""
		'collabname':
			'prefix': 'collabname'
			'body': """
			<collabname>${1}</collabname>
			"""
		'colophon':
			'prefix': 'colophon'
			'body': """
			<colophon id="${1}">
				${2}
			</colophon>
			"""
		'colspec':
			'prefix': 'colspec'
			'body': """
			<colspec colname="${1}" colnum="${2}" colwidth="${3}" />
			"""
		'command':
			'prefix': 'command'
			'body': """
			<command>${1}</command>
			"""
		'computeroutput':
			'prefix': 'computeroutput'
			'body': """
			<computeroutput>${1}</computeroutput>
			"""
		'confdates':
			'prefix': 'confdates'
			'body': """
			<confdates>${1}</confdates>
			"""
		'confgroup':
			'prefix': 'confgroup'
			'body': """
			<confgroup>
				${1}
			</confgroup>
			"""
		'confnum':
			'prefix': 'confnum'
			'body': """
			<confnum>${1}</confnum>
			"""
		'confsponsor':
			'prefix': 'confsponsor'
			'body': """
			<confsponsor>${1}</confsponsor>
			"""
		'conftitle':
			'prefix': 'conftitle'
			'body': """
			<conftitle>${1}</conftitle>
			"""
		'constant':
			'prefix': 'constant'
			'body': """
			<constant>${1}</constant>
			"""
		'constructorsynopsis':
			'prefix': 'constructorsynopsis'
			'body': """
			<constructorsynopsis language="${1}">
				${2}
			</constructorsynopsis>
			"""
		'contractnum':
			'prefix': 'contractnum'
			'body': """
			<contractnum>${1}</contractnum>
			"""
		'contractsponsor':
			'prefix': 'contractsponsor'
			'body': """
			<contractsponsor>${1}</contractsponsor>
			"""
		'contrib':
			'prefix': 'contrib'
			'body': """
			<contrib>${1}</contrib>
			"""
		'copyright':
			'prefix': 'copyright'
			'body': """
			<copyright>
				${1}
			</copyright>
			"""
		'coref':
			'prefix': 'coref'
			'body': """
			<coref label="${1}" linkend="${2}" />
			"""
		'corpauthor':
			'prefix': 'corpauthor'
			'body': """
			<corpauthor>${1}</corpauthor>
			"""
		'corpcredit':
			'prefix': 'corpcredit'
			'body': """
			<corpcredit>${1}</corpcredit>
			"""
		'corpname':
			'prefix': 'corpname'
			'body': """
			<corpname>${1}</corpname>
			"""
		'country':
			'prefix': 'country'
			'body': """
			<country>${1}</country>
			"""
		'database':
			'prefix': 'database'
			'body': """
			<database class="${1}">${2}</database>
			"""
		'date':
			'prefix': 'date'
			'body': """
			<date>${1}</date>
			"""
		'dedication':
			'prefix': 'dedication'
			'body': """
			<dedication>
				${1}
			</dedication>
			"""
		'destructorsynopsis':
			'prefix': 'destructorsynopsis'
			'body': """
			<destructorsynopsis language="${1}">
				${2}
			</destructorsynopsis>
			"""
		'edition':
			'prefix': 'edition'
			'body': """
			<edition>${1}</edition>
			"""
		'editor':
			'prefix': 'editor'
			'body': """
			<editor>
				${1}
			</editor>
			"""
		'email':
			'prefix': 'email'
			'body': """
			<email>${1}</email>
			"""
		'emphasis':
			'prefix': 'emphasis'
			'body': """
			<emphasis>${1}</emphasis>
			"""
		'entry':
			'prefix': 'entry'
			'body': """
			<entry>
				${1}
			</entry>
			"""
		'entrytbl':
			'prefix': 'entrytbl'
			'body': """
			<entrytbl cols="${1}">
				${2}
			</entrytbl>
			"""
		'envar':
			'prefix': 'envar'
			'body': """
			<envar>${1}</envar>
			"""
		'epigraph':
			'prefix': 'epigraph'
			'body': """
			<epigraph>
				${1}
			</epigraph>
			"""
		'equation':
			'prefix': 'equation'
			'body': """
			<equation>
				${1}
			</equation>
			"""
		'errorcode':
			'prefix': 'errorcode'
			'body': """
			<errorcode>${1}</errorcode>
			"""
		'errorname':
			'prefix': 'errorname'
			'body': """
			<errorname>${1}</errorname>
			"""
		'errortext':
			'prefix': 'errortext'
			'body': """
			<errortext>${1}</errortext>
			"""
		'errortype':
			'prefix': 'errortype'
			'body': """
			<errortype>${1}</errortype>
			"""
		'example':
			'prefix': 'example'
			'body': """
			<example id="${1}">
				${2}
			</example>
			"""
		'exceptionname':
			'prefix': 'exceptionname'
			'body': """
			<exceptionname>${1}</exceptionname>
			"""
		'fax':
			'prefix': 'fax'
			'body': """
			<fax>${1}</fax>
			"""
		'fieldsynopsis':
			'prefix': 'fieldsynopsis'
			'body': """
			<fieldsynopsis language="${1}">
				${2}
			</fieldsynopsis>
			"""
		'figure':
			'prefix': 'figure'
			'body': """
			<figure id="${1}">
				${2}
			</figure>
			"""
		'filename':
			'prefix': 'filename'
			'body': """
			<filename>${1}</filename>
			"""
		'firstname':
			'prefix': 'firstname'
			'body': """
			<firstname>${1}</firstname>
			"""
		'firstterm':
			'prefix': 'firstterm'
			'body': """
			<firstterm>${1}</firstterm>
			"""
		'footnote':
			'prefix': 'footnote'
			'body': """
			<footnote>
				${1}
			</footnote>
			"""
		'footnoteref':
			'prefix': 'footnoteref'
			'body': """
			<footnoteref linkend="${1}" />
			"""
		'foreignphrase':
			'prefix': 'foreignphrase'
			'body': """
			<foreignphrase>${1}</foreignphrase>
			"""
		'formalpara':
			'prefix': 'formalpara'
			'body': """
			<formalpara>
				${1}
			</formalpara>
			"""
		'funcdef':
			'prefix': 'funcdef'
			'body': """
			<funcdef>${1}</funcdef>
			"""
		'funcparams':
			'prefix': 'funcparams'
			'body': """
			<funcparams>${1}</funcparams>
			"""
		'funcprototype':
			'prefix': 'funcprototype'
			'body': """
			<funcprototype>
				${1}
			</funcprototype>
			"""
		'funcsynopsis':
			'prefix': 'funcsynopsis'
			'body': """
			<funcsynopsis>
				${1}
			</funcsynopsis>
			"""
		'funcsynopsisinfo':
			'prefix': 'funcsynopsisinfo'
			'body': """
			<funcsynopsisinfo>
				${1}
			</funcsynopsisinfo>
			"""
		'function':
			'prefix': 'function'
			'body': """
			<function>${1}</function>
			"""
		'glossary':
			'prefix': 'glossary'
			'body': """
			<glossary id="${1}">
				${2}
			</glossary>
			"""
		'glossaryinfo':
			'prefix': 'glossaryinfo'
			'body': """
			<glossaryinfo>
				${1}
			</glossaryinfo>
			"""
		'glossdef':
			'prefix': 'glossdef'
			'body': """
			<glossdef>
				${1}
			</glossdef>
			"""
		'glossdiv':
			'prefix': 'glossdiv'
			'body': """
			<glossdiv>
				${1}
			</glossdiv>
			"""
		'glossentry':
			'prefix': 'glossentry'
			'body': """
			<glossentry>
				${1}
			</glossentry>
			"""
		'glosslist':
			'prefix': 'glosslist'
			'body': """
			<glosslist>
				${1}
			</glosslist>
			"""
		'glosssee':
			'prefix': 'glosssee'
			'body': """
			<glosssee otherterm="${1}">${2}</glosssee>
			"""
		'glossseealso':
			'prefix': 'glossseealso'
			'body': """
			<glossseealso otherterm="${1}">${2}</glossseealso>
			"""
		'glossterm':
			'prefix': 'glossterm'
			'body': """
			<glossterm>${1}</glossterm>
			"""
		'graphic':
			'prefix': 'graphic'
			'body': """
			<graphic fileref="${1}" />
			"""
		'graphicco':
			'prefix': 'graphicco'
			'body': """
			<graphicco>
				${1}
			</graphicco>
			"""
		'group':
			'prefix': 'group'
			'body': """
			<group>
				${1}
			</group>
			"""
		'guibutton':
			'prefix': 'guibutton'
			'body': """
			<guibutton>${1}</guibutton>
			"""
		'guiicon':
			'prefix': 'guiicon'
			'body': """
			<guiicon>${1}</guiicon>
			"""
		'guilabel':
			'prefix': 'guilabel'
			'body': """
			<guilabel>${1}</guilabel>
			"""
		'guimenu':
			'prefix': 'guimenu'
			'body': """
			<guimenu>${1}</guimenu>
			"""
		'guimenuitem':
			'prefix': 'guimenuitem'
			'body': """
			<guimenuitem>${1}</guimenuitem>
			"""
		'guisubmenu':
			'prefix': 'guisubmenu'
			'body': """
			<guisubmenu>${1}</guisubmenu>
			"""
		'hardware':
			'prefix': 'hardware'
			'body': """
			<hardware>${1}</hardware>
			"""
		'highlights':
			'prefix': 'highlights'
			'body': """
			<highlights>
				${1}
			</highlights>
			"""
		'holder':
			'prefix': 'holder'
			'body': """
			<holder>${1}</holder>
			"""
		'honorific':
			'prefix': 'honorific'
			'body': """
			<honorific>${1}</honorific>
			"""
		'imagedata':
			'prefix': 'imagedata'
			'body': """
			<imagedata fileref="${1}" format="${2:PNG}" scalefit="${3:0}" />
			"""
		'imageobject':
			'prefix': 'imageobject'
			'body': """
			<imageobject>
				<imagedata fileref="${1}" format="${2:PNG}" scalefit="${3:0}" />
			</imageobject>
			"""
		'imageobjectco':
			'prefix': 'imageobjectco'
			'body': """
			<imageobjectco>
				${1}
			</imageobjectco>
			"""
		'important':
			'prefix': 'important'
			'body': """
			<important>
				${1}
			</important>
			"""
		'index':
			'prefix': 'index'
			'body': """
			<index id="${1}">
				${2}
			</index>
			"""
		'indexdiv':
			'prefix': 'indexdiv'
			'body': """
			<indexdiv>
				${1}
			</indexdiv>
			"""
		'indexentry':
			'prefix': 'indexentry'
			'body': """
			<indexentry>
				${1}
			</indexentry>
			"""
		'indexinfo':
			'prefix': 'indexinfo'
			'body': """
			<indexinfo>
				${1}
			</indexinfo>
			"""
		'indexterm':
			'prefix': 'indexterm'
			'body': """
			<indexterm>
				${1}
			</indexterm>
			"""
		'informalequation':
			'prefix': 'informalequation'
			'body': """
			<informalequation>
				${1}
			</informalequation>
			"""
		'informalexample':
			'prefix': 'informalexample'
			'body': """
			<informalexample>
				${1}
			</informalexample>
			"""
		'informalfigure':
			'prefix': 'informalfigure'
			'body': """
			<informalfigure>
				${1}
			</informalfigure>
			"""
		'informaltable':
			'prefix': 'informaltable'
			'body': """
			<informaltable>
				${1}
			</informaltable>
			"""
		'initializer':
			'prefix': 'initializer'
			'body': """
			<initializer>${1}</initializer>
			"""
		'inlineequation':
			'prefix': 'inlineequation'
			'body': """
			<inlineequation>
				${1}
			</inlineequation>
			"""
		'inlinegraphic':
			'prefix': 'inlinegraphic'
			'body': """
			<inlinegraphic fileref="${1}" format="${2:PNG}" scalefit="${3:0}" />
			"""
		'inlinemediaobject':
			'prefix': 'inlinemediaobject'
			'body': """
			<inlinemediaobject>
				${1}
			</inlinemediaobject>
			"""
		'interface':
			'prefix': 'interface'
			'body': """
			<interface>${1}</interface>
			"""
		'interfacename':
			'prefix': 'interfacename'
			'body': """
			<interfacename>${1}</interfacename>
			"""
		'invpartnumber':
			'prefix': 'invpartnumber'
			'body': """
			<invpartnumber>${1}</invpartnumber>
			"""
		'isbn':
			'prefix': 'isbn'
			'body': """
			<isbn>${1}</isbn>
			"""
		'issn':
			'prefix': 'issn'
			'body': """
			<issn>${1}</issn>
			"""
		'issuenum':
			'prefix': 'issuenum'
			'body': """
			<issuenum>${1}</issuenum>
			"""
		'itemizedlist':
			'prefix': 'itemizedlist'
			'body': """
			<itemizedlist>
				${1}
			</itemizedlist>
			"""
		'itermset':
			'prefix': 'itermset'
			'body': """
			<itermset>
				${1}
			</itermset>
			"""
		'jobtitle':
			'prefix': 'jobtitle'
			'body': """
			<jobtitle>${1}</jobtitle>
			"""
		'keycap':
			'prefix': 'keycap'
			'body': """
			<keycap>${1}</keycap>
			"""
		'keycode':
			'prefix': 'keycode'
			'body': """
			<keycode>${1}</keycode>
			"""
		'keycombo':
			'prefix': 'keycombo'
			'body': """
			<keycombo>${1}</keycombo>
			"""
		'keysym':
			'prefix': 'keysym'
			'body': """
			<keysym>${1}</keysym>
			"""
		'keyword':
			'prefix': 'keyword'
			'body': """
			<keyword>${1}</keyword>
			"""
		'keywordset':
			'prefix': 'keywordset'
			'body': """
			<keywordset>
				${1}
			</keywordset>
			"""
		'label':
			'prefix': 'label'
			'body': """
			<label>${1}</label>
			"""
		'legalnotice':
			'prefix': 'legalnotice'
			'body': """
			<legalnotice>
				${1}
			</legalnotice>
			"""
		'lineage':
			'prefix': 'lineage'
			'body': """
			<lineage>${1}</lineage>
			"""
		'lineannotation':
			'prefix': 'lineannotation'
			'body': """
			<lineannotation>${1}</lineannotation>
			"""
		'link':
			'prefix': 'link'
			'body': """
			<link linkend="${1}">${2}</link>
			"""
		'listitem':
			'prefix': 'listitem'
			'body': """
			<listitem>
				${1}
			</listitem>
			"""
		'literal':
			'prefix': 'literal'
			'body': """
			<literal>${1}</literal>
			"""
		'literallayout':
			'prefix': 'literallayout'
			'body': """
			<literallayout>${1}</literallayout>
			"""
		'lot':
			'prefix': 'lot'
			'body': """
			<lot>
				${1}
			</lot>
			"""
		'lotentry':
			'prefix': 'lotentry'
			'body': """
			<lotentry linkend="${1}">
				${2}
			</lotentry>
			"""
		'manvolnum':
			'prefix': 'manvolnum'
			'body': """
			<manvolnum>${1}</manvolnum>
			"""
		'markup':
			'prefix': 'markup'
			'body': """
			<markup>${1}</markup>
			"""
		'mathphrase':
			'prefix': 'mathphrase'
			'body': """
			<mathphrase>${1}</mathphrase>
			"""
		'medialabel':
			'prefix': 'medialabel'
			'body': """
			<medialabel>${1}</medialabel>
			"""
		'mediaobject':
			'prefix': 'mediaobject'
			'body': """
			<mediaobject>
				${1}
			</mediaobject>
			"""
		'mediaobjectco':
			'prefix': 'mediaobjectco'
			'body': """
			<mediaobjectco>
				${1}
			</mediaobjectco>
			"""
		'member':
			'prefix': 'member'
			'body': """
			<member>
				${1}
			</member>
			"""
		'menuchoice':
			'prefix': 'menuchoice'
			'body': """
			<menuchoice>${1}</menuchoice>
			"""
		'methodname':
			'prefix': 'methodname'
			'body': """
			<methodname>${1}</methodname>
			"""
		'methodparam':
			'prefix': 'methodparam'
			'body': """
			<methodparam>${1}</methodparam>
			"""
		'methodsynopsis':
			'prefix': 'methodsynopsis'
			'body': """
			<methodsynopsis language="${1}">
				${2}
			</methodsynopsis>
			"""
		'modespec':
			'prefix': 'modespec'
			'body': """
			<modespec application="${1}">${2}</modespec>
			"""
		'modifier':
			'prefix': 'modifier'
			'body': """
			<modifier>${1}</modifier>
			"""
		'mousebutton':
			'prefix': 'mousebutton'
			'body': """
			<mousebutton>${1}</mousebutton>
			"""
		'msg':
			'prefix': 'msg'
			'body': """
			<msg>
				${1}
			</msg>
			"""
		'msgaud':
			'prefix': 'msgaud'
			'body': """
			<msgaud>${1}</msgaud>
			"""
		'msgentry':
			'prefix': 'msgentry'
			'body': """
			<msgentry>
				${1}
			</msgentry>
			"""
		'msgexplan':
			'prefix': 'msgexplan'
			'body': """
			<msgexplan>
				${1}
			</msgexplan>
			"""
		'msginfo':
			'prefix': 'msginfo'
			'body': """
			<msginfo>
				${1}
			</msginfo>
			"""
		'msglevel':
			'prefix': 'msglevel'
			'body': """
			<msglevel>${1}</msglevel>
			"""
		'msgmain':
			'prefix': 'msgmain'
			'body': """
			<msgmain>
				${1}
			</msgmain>
			"""
		'msgorig':
			'prefix': 'msgorig'
			'body': """
			<msgorig>${1}</msgorig>
			"""
		'msgrel':
			'prefix': 'msgrel'
			'body': """
			<msgrel>
				${1}
			</msgrel>
			"""
		'msgset':
			'prefix': 'msgset'
			'body': """
			<msgset>
				${1}
			</msgset>
			"""
		'msgsub':
			'prefix': 'msgsub'
			'body': """
			<msgsub>
				${1}
			</msgsub>
			"""
		'msgtext':
			'prefix': 'msgtext'
			'body': """
			<msgtext>
				${1}
			</msgtext>
			"""
		'note':
			'prefix': 'note'
			'body': """
			<note>
				${1}
			</note>
			"""
		'objectinfo':
			'prefix': 'objectinfo'
			'body': """
			<objectinfo>
				${1}
			</objectinfo>
			"""
		'olink':
			'prefix': 'olink'
			'body': """
			<olink targetdocent="${1}">${2}</olink>
			"""
		'ooclass':
			'prefix': 'ooclass'
			'body': """
			<ooclass>${1}</ooclass>
			"""
		'ooexception':
			'prefix': 'ooexception'
			'body': """
			<ooexception>${1}</ooexception>
			"""
		'oointerface':
			'prefix': 'oointerface'
			'body': """
			<oointerface>${1}</oointerface>
			"""
		'option':
			'prefix': 'option'
			'body': """
			<option>${1}</option>
			"""
		'optional':
			'prefix': 'optional'
			'body': """
			<optional>${1}</optional>
			"""
		'orderedlist':
			'prefix': 'orderedlist'
			'body': """
			<orderedlist>
				<listitem>
					${1}
				</listitem>
			</orderedlist>
			"""
		'orgdiv':
			'prefix': 'orgdiv'
			'body': """
			<orgdiv>${1}</orgdiv>
			"""
		'orgname':
			'prefix': 'orgname'
			'body': """
			<orgname>${1}</orgname>
			"""
		'otheraddr':
			'prefix': 'otheraddr'
			'body': """
			<otheraddr>${1}</otheraddr>
			"""
		'othercredit':
			'prefix': 'othercredit'
			'body': """
			<othercredit>
				${1}
			</othercredit>
			"""
		'othername':
			'prefix': 'othername'
			'body': """
			<othername>${1}</othername>
			"""
		'package':
			'prefix': 'package'
			'body': """
			<package>${1}</package>
			"""
		'pagenums':
			'prefix': 'pagenums'
			'body': """
			<pagenums>${1}</pagenums>
			"""
		'para':
			'prefix': 'para'
			'body': """
			<para>
				${1}
			</para>
			"""
		'paramdef':
			'prefix': 'paramdef'
			'body': """
			<paramdef>${1}</paramdef>
			"""
		'parameter':
			'prefix': 'parameter'
			'body': """
			<parameter class="${1:function}">${2}</parameter>
			"""
		'part':
			'prefix': 'part'
			'body': """
			<part id="${1}">
				${2}
			</part>
			"""
		'partinfo':
			'prefix': 'partinfo'
			'body': """
			<partinfo>
				${1}
			</partinfo>
			"""
		'partintro':
			'prefix': 'partintro'
			'body': """
			<partintro>
				${1}
			</partintro>
			"""
		'personblurb':
			'prefix': 'personblurb'
			'body': """
			<personblurb>
				${1}
			</personblurb>
			"""
		'personname':
			'prefix': 'personname'
			'body': """
			<personname>${1}</personname>
			"""
		'phone':
			'prefix': 'phone'
			'body': """
			<phone>${1}</phone>
			"""
		'phrase':
			'prefix': 'phrase'
			'body': """
			<phrase>${1}</phrase>
			"""
		'pob':
			'prefix': 'pob'
			'body': """
			<pob>${1}</pob>
			"""
		'postcode':
			'prefix': 'postcode'
			'body': """
			<postcode>${1}</postcode>
			"""
		'preface':
			'prefix': 'preface'
			'body': """
			<preface id="${1}">
				${2}
			</preface>
			"""
		'prefaceinfo':
			'prefix': 'prefaceinfo'
			'body': """
			<prefaceinfo>
				${1}
			</prefaceinfo>
			"""
		'primary':
			'prefix': 'primary'
			'body': """
			<primary>${1}</primary>
			"""
		'primaryie':
			'prefix': 'primaryie'
			'body': """
			<primaryie>${1}</primaryie>
			"""
		'printhistory':
			'prefix': 'printhistory'
			'body': """
			<printhistory>
				${1}
			</printhistory>
			"""
		'procedure':
			'prefix': 'procedure'
			'body': """
			<procedure id="${1}">
				${2}
			</procedure>
			"""
		'productname':
			'prefix': 'productname'
			'body': """
			<productname class="${1:trade}">${2}</productname>
			"""
		'productnumber':
			'prefix': 'productnumber'
			'body': """
			<productnumber>${1}</productnumber>
			"""
		'programlisting':
			'prefix': 'programlisting'
			'body': """
			<programlisting language="${1}">${2}</programlisting>
			"""
		'programlistingco':
			'prefix': 'programlistingco'
			'body': """
			<programlistingco>
				${1}
			</programlistingco>
			"""
		'prompt':
			'prefix': 'prompt'
			'body': """
			<prompt>${1}</prompt>
			"""
		'property':
			'prefix': 'property'
			'body': """
			<property>${1}</property>
			"""
		'pubdate':
			'prefix': 'pubdate'
			'body': """
			<pubdate>${1}</pubdate>
			"""
		'publisher':
			'prefix': 'publisher'
			'body': """
			<publisher>
				${1}
			</publisher>
			"""
		'publishername':
			'prefix': 'publishername'
			'body': """
			<publishername>${1}</publishername>
			"""
		'pubsnumber':
			'prefix': 'pubsnumber'
			'body': """
			<pubsnumber>${1}</pubsnumber>
			"""
		'qandadiv':
			'prefix': 'qandadiv'
			'body': """
			<qandadiv>
				${1}
			</qandadiv>
			"""
		'qandaentry':
			'prefix': 'qandaentry'
			'body': """
			<qandaentry>
				${1}
			</qandaentry>
			"""
		'qandaset':
			'prefix': 'qandaset'
			'body': """
			<qandaset>
				${1}
			</qandaset>
			"""
		'question':
			'prefix': 'question'
			'body': """
			<question>
				${1}
			</question>
			"""
		'quote':
			'prefix': 'quote'
			'body': """
			<quote>${1}</quote>
			"""
		'refclass':
			'prefix': 'refclass'
			'body': """
			<refclass>${1}</refclass>
			"""
		'refdescriptor':
			'prefix': 'refdescriptor'
			'body': """
			<refdescriptor>${1}</refdescriptor>
			"""
		'refentry':
			'prefix': 'refentry'
			'body': """
			<refentry>
				${1}
			</refentry>
			"""
		'refentryinfo':
			'prefix': 'refentryinfo'
			'body': """
			<refentryinfo>
				${1}
			</refentryinfo>
			"""
		'refentrytitle':
			'prefix': 'refentrytitle'
			'body': """
			<refentrytitle>${1}</refentrytitle>
			"""
		'reference':
			'prefix': 'reference'
			'body': """
			<reference>
				${1}
			</reference>
			"""
		'referenceinfo':
			'prefix': 'referenceinfo'
			'body': """
			<referenceinfo>
				${1}
			</referenceinfo>
			"""
		'refmeta':
			'prefix': 'refmeta'
			'body': """
			<refmeta>
				${1}
			</refmeta>
			"""
		'refmiscinfo':
			'prefix': 'refmiscinfo'
			'body': """
			<refmiscinfo>
				${1}
			</refmiscinfo>
			"""
		'refname':
			'prefix': 'refname'
			'body': """
			<refname>${1}</refname>
			"""
		'refnamediv':
			'prefix': 'refnamediv'
			'body': """
			<refnamediv>
				${1}
			</refnamediv>
			"""
		'refpurpose':
			'prefix': 'refpurpose'
			'body': """
			<refpurpose>${1}</refpurpose>
			"""
		'refsect1':
			'prefix': 'refsect1'
			'body': """
			<refsect1 id="${1}">
				${2}
			</refsect1>
			"""
		'refsect1info':
			'prefix': 'refsect1info'
			'body': """
			<refsect1info>
				${1}
			</refsect1info>
			"""
		'refsect2':
			'prefix': 'refsect2'
			'body': """
			<refsect2 id="${1}">
				${2}
			</refsect2>
			"""
		'refsect2info':
			'prefix': 'refsect2info'
			'body': """
			<refsect2info>
				${1}
			</refsect2info>
			"""
		'refsect3':
			'prefix': 'refsect3'
			'body': """
			<refsect3 id="${1}">
				${2}
			</refsect3>
			"""
		'refsect3info':
			'prefix': 'refsect3info'
			'body': """
			<refsect3info>
				${1}
			</refsect3info>
			"""
		'refsection':
			'prefix': 'refsection'
			'body': """
			<refsection id="${1}">
				${2}
			</refsection>
			"""
		'refsectioninfo':
			'prefix': 'refsectioninfo'
			'body': """
			<refsectioninfo>
				${1}
			</refsectioninfo>
			"""
		'refsynopsisdiv':
			'prefix': 'refsynopsisdiv'
			'body': """
			<refsynopsisdiv>
				${1}
			</refsynopsisdiv>
			"""
		'refsynopsisdivinfo':
			'prefix': 'refsynopsisdivinfo'
			'body': """
			<refsynopsisdivinfo>
				${1}
			</refsynopsisdivinfo>
			"""
		'releaseinfo':
			'prefix': 'releaseinfo'
			'body': """
			<releaseinfo>${1}</releaseinfo>
			"""
		'remark':
			'prefix': 'remark'
			'body': """
			<remark>${1}</remark>
			"""
		'replaceable':
			'prefix': 'replaceable'
			'body': """
			<replaceable>${1}</replaceable>
			"""
		'returnvalue':
			'prefix': 'returnvalue'
			'body': """
			<returnvalue>${1}</returnvalue>
			"""
		'revdescription':
			'prefix': 'revdescription'
			'body': """
			<revdescription>
				${1}
			</revdescription>
			"""
		'revhistory':
			'prefix': 'revhistory'
			'body': """
			<revhistory>
				${1}
			</revhistory>
			"""
		'revision':
			'prefix': 'revision'
			'body': """
			<revision>
				${1}
			</revision>
			"""
		'revnumber':
			'prefix': 'revnumber'
			'body': """
			<revnumber>${1}</revnumber>
			"""
		'revremark':
			'prefix': 'revremark'
			'body': """
			<revremark>${1}</revremark>
			"""
		'row':
			'prefix': 'row'
			'body': """
			<row>
				${1}
			</row>
			"""
		'sbr':
			'prefix': 'sbr'
			'body': """
			<sbr />
			"""
		'screen':
			'prefix': 'screen'
			'body': """
			<screen>${1}</screen>
			"""
		'screenco':
			'prefix': 'screenco'
			'body': """
			<screenco>
				${1}
			</screenco>
			"""
		'screeninfo':
			'prefix': 'screeninfo'
			'body': """
			<screeninfo>${1}</screeninfo>
			"""
		'screenshot':
			'prefix': 'screenshot'
			'body': """
			<screenshot>
				${1}
			</screenshot>
			"""
		'secondary':
			'prefix': 'secondary'
			'body': """
			<secondary>${1}</secondary>
			"""
		'secondaryie':
			'prefix': 'secondaryie'
			'body': """
			<secondaryie>${1}</secondaryie>
			"""
		'sect1':
			'prefix': 'sect1'
			'body': """
			<sect1 id="${1}">
				${2}
			</sect1>
			"""
		'sect1info':
			'prefix': 'sect1info'
			'body': """
			<sect1info>
				${1}
			</sect1info>
			"""
		'sect2':
			'prefix': 'sect2'
			'body': """
			<sect2 id="${1}">
				${2}
			</sect2>
			"""
		'sect2info':
			'prefix': 'sect2info'
			'body': """
			<sect2info>
				${1}
			</sect2info>
			"""
		'sect3':
			'prefix': 'sect3'
			'body': """
			<sect3 id="${1}">
				${2}
			</sect3>
			"""
		'sect3info':
			'prefix': 'sect3info'
			'body': """
			<sect3info>
				${1}
			</sect3info>
			"""
		'sect4':
			'prefix': 'sect4'
			'body': """
			<sect4 id="${1}">
				${2}
			</sect4>
			"""
		'sect4info':
			'prefix': 'sect4info'
			'body': """
			<sect4info>
				${1}
			</sect4info>
			"""
		'sect5':
			'prefix': 'sect5'
			'body': """
			<sect5 id="${1}">
				${2}
			</sect5>
			"""
		'sect5info':
			'prefix': 'sect5info'
			'body': """
			<sect5info>
				${1}
			</sect5info>
			"""
		'section':
			'prefix': 'section'
			'body': """
			<section id="${1}">
				${2}
			</section>
			"""
		'sectioninfo':
			'prefix': 'sectioninfo'
			'body': """
			<sectioninfo>
				${1}
			</sectioninfo>
			"""
		'see':
			'prefix': 'see'
			'body': """
			<see>${1}</see>
			"""
		'seealso':
			'prefix': 'seealso'
			'body': """
			<seealso>${1}</seealso>
			"""
		'seealsoie':
			'prefix': 'seealsoie'
			'body': """
			<seealsoie>${1}</seealsoie>
			"""
		'seeie':
			'prefix': 'seeie'
			'body': """
			<seeie>${1}</seeie>
			"""
		'seg':
			'prefix': 'seg'
			'body': """
			<seg>${1}</seg>
			"""
		'seglistitem':
			'prefix': 'seglistitem'
			'body': """
			<seglistitem>
				${1}
			</seglistitem>
			"""
		'segmentedlist':
			'prefix': 'segmentedlist'
			'body': """
			<segmentedlist>
				${1}
			</segmentedlist>
			"""
		'segtitle':
			'prefix': 'segtitle'
			'body': """
			<segtitle>${1}</segtitle>
			"""
		'seriesvolnums':
			'prefix': 'seriesvolnums'
			'body': """
			<seriesvolnums>${1}</seriesvolnums>
			"""
		'set':
			'prefix': 'set'
			'body': """
			<set>
				${1}
			</set>
			"""
		'setindex':
			'prefix': 'setindex'
			'body': """
			<setindex>
				${1}
			</setindex>
			"""
		'setindexinfo':
			'prefix': 'setindexinfo'
			'body': """
			<setindexinfo>
				${1}
			</setindexinfo>
			"""
		'setinfo':
			'prefix': 'setinfo'
			'body': """
			<setinfo>
				${1}
			</setinfo>
			"""
		'sgmltag':
			'prefix': 'sgmltag'
			'body': """
			<sgmltag>${1}</sgmltag>
			"""
		'shortaffil':
			'prefix': 'shortaffil'
			'body': """
			<shortaffil>${1}</shortaffil>
			"""
		'shortcut':
			'prefix': 'shortcut'
			'body': """
			<shortcut>${1}</shortcut>
			"""
		'sidebar':
			'prefix': 'sidebar'
			'body': """
			<sidebar>
				${1}
			</sidebar>
			"""
		'sidebarinfo':
			'prefix': 'sidebarinfo'
			'body': """
			<sidebarinfo>
				${1}
			</sidebarinfo>
			"""
		'simpara':
			'prefix': 'simpara'
			'body': """
			<simpara>
				${1}
			</simpara>
			"""
		'simplelist':
			'prefix': 'simplelist'
			'body': """
			<simplelist>
				${1}
			</simplelist>
			"""
		'simplemsgentry':
			'prefix': 'simplemsgentry'
			'body': """
			<simplemsgentry>
				${1}
			</simplemsgentry>
			"""
		'simplesect':
			'prefix': 'simplesect'
			'body': """
			<simplesect id="${1}">
				${2}
			</simplesect>
			"""
		'spanspec':
			'prefix': 'spanspec'
			'body': """
			<spanspec spanname="${1}" namest="${2}" nameend="${3}" />
			"""
		'state':
			'prefix': 'state'
			'body': """
			<state>${1}</state>
			"""
		'step':
			'prefix': 'step'
			'body': """
			<step>
				${1}
			</step>
			"""
		'stepalternatives':
			'prefix': 'stepalternatives'
			'body': """
			<stepalternatives>
				${1}
			</stepalternatives>
			"""
		'street':
			'prefix': 'street'
			'body': """
			<street>${1}</street>
			"""
		'structfield':
			'prefix': 'structfield'
			'body': """
			<structfield>${1}</structfield>
			"""
		'structname':
			'prefix': 'structname'
			'body': """
			<structname>${1}</structname>
			"""
		'subject':
			'prefix': 'subject'
			'body': """
			<subject>
				${1}
			</subject>
			"""
		'subjectset':
			'prefix': 'subjectset'
			'body': """
			<subjectset>
				${1}
			</subjectset>
			"""
		'subjectterm':
			'prefix': 'subjectterm'
			'body': """
			<subjectterm>${1}</subjectterm>
			"""
		'subscript':
			'prefix': 'subscript'
			'body': """
			<subscript>${1}</subscript>
			"""
		'substeps':
			'prefix': 'substeps'
			'body': """
			<substeps>
				${1}
			</substeps>
			"""
		'subtitle':
			'prefix': 'subtitle'
			'body': """
			<subtitle>${1}</subtitle>
			"""
		'superscript':
			'prefix': 'superscript'
			'body': """
			<superscript>${1}</superscript>
			"""
		'surname':
			'prefix': 'surname'
			'body': """
			<surname>${1}</surname>
			"""
		'symbol':
			'prefix': 'symbol'
			'body': """
			<symbol>${1}</symbol>
			"""
		'synopfragment':
			'prefix': 'synopfragment'
			'body': """
			<synopfragment id="${1}">
				${2}
			</synopfragment>
			"""
		'synopfragmentref':
			'prefix': 'synopfragmentref'
			'body': """
			<synopfragmentref linkend="${1}">
				${2}
			</synopfragmentref>
			"""
		'synopsis':
			'prefix': 'synopsis'
			'body': """
			<synopsis>${1}</synopsis>
			"""
		'systemitem':
			'prefix': 'systemitem'
			'body': """
			<systemitem>${1}</systemitem>
			"""
		'table':
			'prefix': 'table'
			'body': """
			<table id="${1}">
				${2}
			</table>
			"""
		'task':
			'prefix': 'task'
			'body': """
			<task id="${1}">
				${2}
			</task>
			"""
		'taskprerequisites':
			'prefix': 'taskprerequisites'
			'body': """
			<taskprerequisites>
				${1}
			</taskprerequisites>
			"""
		'taskrelated':
			'prefix': 'taskrelated'
			'body': """
			<taskrelated>
				${1}
			</taskrelated>
			"""
		'tasksummary':
			'prefix': 'tasksummary'
			'body': """
			<tasksummary>
				${1}
			</tasksummary>
			"""
		'tbody':
			'prefix': 'tbody'
			'body': """
			<tbody>
				${1}
			</tbody>
			"""
		'td':
			'prefix': 'td'
			'body': """
			<td>
				${1}
			</td>
			"""
		'term':
			'prefix': 'term'
			'body': """
			<term>${1}</term>
			"""
		'termdef':
			'prefix': 'termdef'
			'body': """
			<termdef>${1}</termdef>
			"""
		'tertiary':
			'prefix': 'tertiary'
			'body': """
			<tertiary>${1}</tertiary>
			"""
		'tertiaryie':
			'prefix': 'tertiaryie'
			'body': """
			<tertiaryie>${1}</tertiaryie>
			"""
		'textdata':
			'prefix': 'textdata'
			'body': """
			<textdata fileref="${1}" />
			"""
		'textobject':
			'prefix': 'textobject'
			'body': """
			<textobject>
				${1}
			</textobject>
			"""
		'tfoot':
			'prefix': 'tfoot'
			'body': """
			<tfoot>
				${1}
			</tfoot>
			"""
		'tgroup':
			'prefix': 'tgroup'
			'body': """
			<tgroup cols="${1}">
				${2}
			</tgroup>
			"""
		'th':
			'prefix': 'th'
			'body': """
			<th>
				${1}
			</th>
			"""
		'thead':
			'prefix': 'thead'
			'body': """
			<thead>
				${1}
			</thead>
			"""
		'tip':
			'prefix': 'tip'
			'body': """
			<tip>
				${1}
			</tip>
			"""
		'title':
			'prefix': 'title'
			'body': """
			<title>${1}</title>
			"""
		'titleabbrev':
			'prefix': 'titleabbrev'
			'body': """
			<titleabbrev>${1}</titleabbrev>
			"""
		'toc':
			'prefix': 'toc'
			'body': """
			<toc>
				${1}
			</toc>
			"""
		'tocback':
			'prefix': 'tocback'
			'body': """
			<tocback linkend="${1}">${2}</tocback>
			"""
		'tocchap':
			'prefix': 'tocchap'
			'body': """
			<tocchap>
				${1}
			</tocchap>
			"""
		'tocentry':
			'prefix': 'tocentry'
			'body': """
			<tocentry linkend="${1}">${2}</tocentry>
			"""
		'tocfront':
			'prefix': 'tocfront'
			'body': """
			<tocfront linkend="${1}">${2}</tocfront>
			"""
		'toclevel1':
			'prefix': 'toclevel1'
			'body': """
			<toclevel1>
				${1}
			</toclevel1>
			"""
		'toclevel2':
			'prefix': 'toclevel2'
			'body': """
			<toclevel2>
				${1}
			</toclevel2>
			"""
		'toclevel3':
			'prefix': 'toclevel3'
			'body': """
			<toclevel3>
				${1}
			</toclevel3>
			"""
		'toclevel4':
			'prefix': 'toclevel4'
			'body': """
			<toclevel4>
				${1}
			</toclevel4>
			"""
		'toclevel5':
			'prefix': 'toclevel5'
			'body': """
			<toclevel5>
				${1}
			</toclevel5>
			"""
		'tocpart':
			'prefix': 'tocpart'
			'body': """
			<tocpart>
				${1}
			</tocpart>
			"""
		'token':
			'prefix': 'token'
			'body': """
			<token>${1}</token>
			"""
		'tr':
			'prefix': 'tr'
			'body': """
			<tr>
				${1}
			</tr>
			"""
		'trademark':
			'prefix': 'trademark'
			'body': """
			<trademark class="${1:trade}">${2}</trademark>
			"""
		'type':
			'prefix': 'type'
			'body': """
			<type>${1}</type>
			"""
		'ulink':
			'prefix': 'ulink'
			'body': """
			<ulink url="${1}">${2}</ulink>
			"""
		'uri':
			'prefix': 'uri'
			'body': """
			<uri>${1}</uri>
			"""
		'userinput':
			'prefix': 'userinput'
			'body': """
			<userinput>${1}</userinput>
			"""
		'varargs':
			'prefix': 'varargs'
			'body': """
			<varargs />
			"""
		'variablelist':
			'prefix': 'variablelist'
			'body': """
			<variablelist>
				${1}
			</variablelist>
			"""
		'varlistentry':
			'prefix': 'varlistentry'
			'body': """
			<varlistentry>
				${1}
			</varlistentry>
			"""
		'varname':
			'prefix': 'varname'
			'body': """
			<varname>${1}</varname>
			"""
		'videodata':
			'prefix': 'videodata'
			'body': """
			<videodata fileref="${1}" scalefit="${2:0}" />
			"""
		'videoobject':
			'prefix': 'videoobject'
			'body': """
			<videoobject>
				${1}
			</videoobject>
			"""
		'void':
			'prefix': 'void'
			'body': """
			<void />
			"""
		'volumenum':
			'prefix': 'volumenum'
			'body': """
			<volumenum>${1}</volumenum>
			"""
		'warning':
			'prefix': 'warning'
			'body': """
			<warning>
				${1}
			</warning>
			"""
		'wordasword':
			'prefix': 'wordasword'
			'body': """
			<wordasword>${1}</wordasword>
			"""
		'xref':
			'prefix': 'xref'
			'body': """
			<xref linkend="${1}" />
			"""
		'year':
			'prefix': 'year'
			'body': """
			<year>${1}</year>
			"""
		'bold':
			'prefix': 'bold'
			'body': """
			<emphasis role="bold">${1}</emphasis>
			"""
		'strong':
			'prefix': 'strong'
			'body': """
			<emphasis role="strong">${1}</emphasis>
			"""
		'devicefile':
			'prefix': 'devicefile'
			'body': """
			<filename class="devicefile">${1}</filename>
			"""
		'directory':
			'prefix': 'directory'
			'body': """
			<filename class="directory">${1}</filename>
			"""
		'extension':
			'prefix': 'extension'
			'body': """
			<filename class="extension">${1}</filename>
			"""
		'headerfile':
			'prefix': 'headerfile'
			'body': """
			<filename class="headerfile">${1}</filename>
			"""
		'libraryfile':
			'prefix': 'libraryfile'
			'body': """
			<filename class="libraryfile">${1}</filename>
			"""
		'partition':
			'prefix': 'partition'
			'body': """
			<filename class="partition">${1}</filename>
			"""
		'symlink':
			'prefix': 'symlink'
			'body': """
			<filename class="symlink">${1}</filename>
			"""
		'cartridge':
			'prefix': 'cartridge'
			'body': """
			<medialabel class="cartridge">${1}</medialabel>
			"""
		'cdrom':
			'prefix': 'cdrom'
			'body': """
			<medialabel class="cdrom">${1}</medialabel>
			"""
		'disk':
			'prefix': 'disk'
			'body': """
			<medialabel class="disk">${1}</medialabel>
			"""
		'tape':
			'prefix': 'tape'
			'body': """
			<medialabel class="tape">${1}</medialabel>
			"""
		'daemon':
			'prefix': 'daemon'
			'body': """
			<systemitem class="daemon">${1}</systemitem>
			"""
		'domainname':
			'prefix': 'domainname'
			'body': """
			<systemitem class="domainname">${1}</systemitem>
			"""
		'etheraddress':
			'prefix': 'etheraddress'
			'body': """
			<systemitem class="etheraddress">${1}</systemitem>
			"""
		'eventhandler':
			'prefix': 'eventhandler'
			'body': """
			<systemitem class="eventhandler">${1}</systemitem>
			"""
		'event':
			'prefix': 'event'
			'body': """
			<systemitem class="event">${1}</systemitem>
			"""
		'filesystem':
			'prefix': 'filesystem'
			'body': """
			<systemitem class="filesystem">${1}</systemitem>
			"""
		'fqdomainname':
			'prefix': 'fqdomainname'
			'body': """
			<systemitem class="fqdomainname">${1}</systemitem>
			"""
		'groupname':
			'prefix': 'groupname'
			'body': """
			<systemitem class="groupname">${1}</systemitem>
			"""
		'ipaddress':
			'prefix': 'ipaddress'
			'body': """
			<systemitem class="ipaddress">${1}</systemitem>
			"""
		'library':
			'prefix': 'library'
			'body': """
			<systemitem class="library">${1}</systemitem>
			"""
		'macro':
			'prefix': 'macro'
			'body': """
			<systemitem class="macro">${1}</systemitem>
			"""
		'netmask':
			'prefix': 'netmask'
			'body': """
			<systemitem class="netmask">${1}</systemitem>
			"""
		'newsgroup':
			'prefix': 'newsgroup'
			'body': """
			<systemitem class="newsgroup">${1}</systemitem>
			"""
		'osname':
			'prefix': 'osname'
			'body': """
			<systemitem class="osname">${1}</systemitem>
			"""
		'process':
			'prefix': 'process'
			'body': """
			<systemitem class="process">${1}</systemitem>
			"""
		'protocol':
			'prefix': 'protocol'
			'body': """
			<systemitem class="protocol">${1}</systemitem>
			"""
		'resource':
			'prefix': 'resource'
			'body': """
			<systemitem class="resource">${1}</systemitem>
			"""
		'server':
			'prefix': 'server'
			'body': """
			<systemitem class="server">${1}</systemitem>
			"""
		'service':
			'prefix': 'service'
			'body': """
			<systemitem class="service">${1}</systemitem>
			"""
		'systemname':
			'prefix': 'systemname'
			'body': """
			<systemitem class="systemname">${1}</systemitem>
			"""
		'username':
			'prefix': 'username'
			'body': """
			<systemitem class="username">${1}</systemitem>
			"""
		'xi:include':
			'prefix': 'xi:include'
			'body': """
			<xi:include href="${1}.xml" xmlns:xi="http://www.w3.org/2001/XInclude" />
			"""
		'xi:fallback':
			'prefix': 'xi:fallback'
			'body': """
			<xi:fallback xmlns:xi="http://www.w3.org/2001/XInclude">
				${1}
			</xi:fallback>
			"""
		'xml':
			'prefix': 'xml'
			'body': """
			<?xml version='${1:1.0}' encoding='${2:utf-8}' ?>
			"""
		'doctype':
			'prefix': 'doctype'
			'body': """
			<!DOCTYPE ${1:chapter} PUBLIC "-//OASIS//DTD DocBook XML V4.5//EN" "http://www.oasis-open.org/docbook/xml/4.5/docbookx.dtd">
			"""
		'cdata':
			'prefix': 'cdata'
			'body': """
			<![CDATA[${1}]]>
	    """
```
