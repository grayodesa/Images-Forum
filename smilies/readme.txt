HACK NAME : SUPER SMILIES HACK by SAL2000

VERSION: 1.0 - 03/08/2000

DESCRIPTION : The purpose of this hack is to have a smiley hack that doesn't consume much cpoo time yet allows
users to post smilies with ease.
you must have ubb images turned on in order to work.

AUTHOR : SAL2000 , CWM
PROPOSED BY : CWM
ORINGAL HACK : CWM'S SMILIE HACK (http://smilecwm.tripod.com/smileyhack.zip)
DEMO : 
CREDITS : CWM for the Great Idea :)

If you feel you have contributed but not been given credit please email me - leshrac@magictraders.com

REQUIREMENTS :	A full version of the UBB.
                This version has only been tested to work on UBB v5.44. It may work on slightly earlier versions, but has not been tested.

DOWNLOAD URL : http://www.rdpc.net/sshack.zip


SUPPORT : wondergroup@uol.com.br


INSTALLATION INSTRUCTIONS:

the only file to be hacked is the postings.cgi, so back it up and get ready to hack it.

First, make a folder in your NonCGI Directory called 'smilies', then upload cwm1.gif - cwm45.gif
and the smileymap.gif into that folder.

----------
Find this:
----------

if ($AllowIcons eq "TRUE") {
$IconWording = &IconFieldHTML;
}  else {
$IconWording = "";
}

----------------------
And under it put this:
----------------------

if ($UBBImages eq "ON") {
$SmileMapper = qq(<img src=$NonCGIURL/smilies/smileymap.gif usemap="#Smile" border=0><MAP NAME="Smile">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm1.gif[/IMG] ';" COORDS="8,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm2.gif[/IMG] ';" COORDS="25,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm3.gif[/IMG] ';" COORDS="42,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm4.gif[/IMG] ';" COORDS="59,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm5.gif[/IMG] ';" COORDS="76,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm6.gif[/IMG] ';" COORDS="8,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm7.gif[/IMG] ';" COORDS="25,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm8.gif[/IMG] ';" COORDS="42,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm9.gif[/IMG] ';" COORDS="59,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm10.gif[/IMG] ';" COORDS="76,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm11.gif[/IMG] ';" COORDS="8,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm12.gif[/IMG] ';" COORDS="25,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm13.gif[/IMG] ';" COORDS="42,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm14.gif[/IMG] ';" COORDS="59,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm15.gif[/IMG] ';" COORDS="76,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm16.gif[/IMG] ';" COORDS="8,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm17.gif[/IMG] ';" COORDS="25,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm18.gif[/IMG] ';" COORDS="42,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm19.gif[/IMG] ';" COORDS="59,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm20.gif[/IMG] ';" COORDS="76,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm21.gif[/IMG] ';" COORDS="8,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm22.gif[/IMG] ';" COORDS="25,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm23.gif[/IMG] ';" COORDS="42,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm24.gif[/IMG] ';" COORDS="59,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm25.gif[/IMG] ';" COORDS="76,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm26.gif[/IMG] ';" COORDS="8,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm27.gif[/IMG] ';" COORDS="25,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm28.gif[/IMG] ';" COORDS="42,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm29.gif[/IMG] ';" COORDS="59,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm30.gif[/IMG] ';" COORDS="76,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm31.gif[/IMG] ';" COORDS="8,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm32.gif[/IMG] ';" COORDS="25,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm33.gif[/IMG] ';" COORDS="42,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm34.gif[/IMG] ';" COORDS="59,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm35.gif[/IMG] ';" COORDS="76,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm36.gif[/IMG] ';" COORDS="8,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm37.gif[/IMG] ';" COORDS="25,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm38.gif[/IMG] ';" COORDS="42,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm39.gif[/IMG] ';" COORDS="59,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm40.gif[/IMG] ';" COORDS="76,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm41.gif[/IMG] ';" COORDS="8,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm42.gif[/IMG] ';" COORDS="25,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm43.gif[/IMG] ';" COORDS="42,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm44.gif[/IMG] ';" COORDS="59,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.ReplyMessage.value+='[IMG]$NonCGIURL/smilies/cwm45.gif[/IMG] ';" COORDS="76,145,8">
<AREA SHAPE="rec" href="http://smilecwm.tripod.com/" Target="_blank" Coords="0,153,85,170"><AREA SHAPE="default" NOHREF>
</MAP>);
}

----------
Find this:
----------

$SmiliesLink</font>

----------------
Replace it with:
----------------

$SmiliesLink</font><br>$SmileMapper

----------
Find this:
----------

if ($AllowIcons eq "TRUE") {
$IconWording = &IconFieldHTML;
}  else {
$IconWording = "";
}

----------------------
And under it put this:
----------------------

if ($UBBImages eq "ON") {
$SmileMapper = qq(<img src=$NonCGIURL/smilies/smileymap.gif usemap="#Smile" border=0><MAP NAME="Smile">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm1.gif[/IMG] ';" COORDS="8,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm2.gif[/IMG] ';" COORDS="25,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm3.gif[/IMG] ';" COORDS="42,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm4.gif[/IMG] ';" COORDS="59,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm5.gif[/IMG] ';" COORDS="76,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm6.gif[/IMG] ';" COORDS="8,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm7.gif[/IMG] ';" COORDS="25,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm8.gif[/IMG] ';" COORDS="42,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm9.gif[/IMG] ';" COORDS="59,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm10.gif[/IMG] ';" COORDS="76,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm11.gif[/IMG] ';" COORDS="8,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm12.gif[/IMG] ';" COORDS="25,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm13.gif[/IMG] ';" COORDS="42,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm14.gif[/IMG] ';" COORDS="59,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm15.gif[/IMG] ';" COORDS="76,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm16.gif[/IMG] ';" COORDS="8,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm17.gif[/IMG] ';" COORDS="25,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm18.gif[/IMG] ';" COORDS="42,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm19.gif[/IMG] ';" COORDS="59,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm20.gif[/IMG] ';" COORDS="76,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm21.gif[/IMG] ';" COORDS="8,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm22.gif[/IMG] ';" COORDS="25,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm23.gif[/IMG] ';" COORDS="42,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm24.gif[/IMG] ';" COORDS="59,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm25.gif[/IMG] ';" COORDS="76,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm26.gif[/IMG] ';" COORDS="8,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm27.gif[/IMG] ';" COORDS="25,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm28.gif[/IMG] ';" COORDS="42,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm29.gif[/IMG] ';" COORDS="59,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm30.gif[/IMG] ';" COORDS="76,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm31.gif[/IMG] ';" COORDS="8,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm32.gif[/IMG] ';" COORDS="25,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm33.gif[/IMG] ';" COORDS="42,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm34.gif[/IMG] ';" COORDS="59,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm35.gif[/IMG] ';" COORDS="76,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm36.gif[/IMG] ';" COORDS="8,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm37.gif[/IMG] ';" COORDS="25,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm38.gif[/IMG] ';" COORDS="42,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm39.gif[/IMG] ';" COORDS="59,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm40.gif[/IMG] ';" COORDS="76,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm41.gif[/IMG] ';" COORDS="8,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm42.gif[/IMG] ';" COORDS="25,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm43.gif[/IMG] ';" COORDS="42,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm44.gif[/IMG] ';" COORDS="59,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.PostTopic.Message.value+='[IMG]$NonCGIURL/smilies/cwm45.gif[/IMG] ';" COORDS="76,145,8">
<AREA SHAPE="rec" href="http://smilecwm.tripod.com/" Target="_blank" Coords="0,153,85,170">
<AREA SHAPE="default" NOHREF></MAP>);
}

----------
Find this:
----------

$SmiliesLink</font>

----------------
Replace it with:
----------------

$SmiliesLink</font><br>$SmileMapper

----------
Find this:
----------

if ($in{'ReplyNum'} eq "000000") {
	$WarningWords = "Note: deleting this post will result in the deletion of the entire topic, since this post is the first post in the topic.";
}

----------------------
And under it put this:
----------------------

if ($UBBImages eq "ON") {
$SmileMapper = qq(<img src=$NonCGIURL/smilies/smileymap.gif usemap="#Smile" border=0><MAP NAME="Smile">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm1.gif[/IMG] ';" COORDS="8,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm2.gif[/IMG] ';" COORDS="25,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm3.gif[/IMG] ';" COORDS="42,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm4.gif[/IMG] ';" COORDS="59,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm5.gif[/IMG] ';" COORDS="76,8,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm6.gif[/IMG] ';" COORDS="8,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm7.gif[/IMG] ';" COORDS="25,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm8.gif[/IMG] ';" COORDS="42,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm9.gif[/IMG] ';" COORDS="59,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm10.gif[/IMG] ';" COORDS="76,25,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm11.gif[/IMG] ';" COORDS="8,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm12.gif[/IMG] ';" COORDS="25,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm13.gif[/IMG] ';" COORDS="42,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm14.gif[/IMG] ';" COORDS="59,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm15.gif[/IMG] ';" COORDS="76,42,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm16.gif[/IMG] ';" COORDS="8,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm17.gif[/IMG] ';" COORDS="25,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm18.gif[/IMG] ';" COORDS="42,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm19.gif[/IMG] ';" COORDS="59,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm20.gif[/IMG] ';" COORDS="76,59,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm21.gif[/IMG] ';" COORDS="8,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm22.gif[/IMG] ';" COORDS="25,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm23.gif[/IMG] ';" COORDS="42,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm24.gif[/IMG] ';" COORDS="59,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm25.gif[/IMG] ';" COORDS="76,76,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm26.gif[/IMG] ';" COORDS="8,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm27.gif[/IMG] ';" COORDS="25,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm28.gif[/IMG] ';" COORDS="42,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm29.gif[/IMG] ';" COORDS="59,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm30.gif[/IMG] ';" COORDS="76,94,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm31.gif[/IMG] ';" COORDS="8,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm32.gif[/IMG] ';" COORDS="25,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm33.gif[/IMG] ';" COORDS="42,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm34.gif[/IMG] ';" COORDS="59,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm35.gif[/IMG] ';" COORDS="76,110,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm36.gif[/IMG] ';" COORDS="8,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm37.gif[/IMG] ';" COORDS="25,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm38.gif[/IMG] ';" COORDS="42,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm39.gif[/IMG] ';" COORDS="59,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm40.gif[/IMG] ';" COORDS="76,128,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm41.gif[/IMG] ';" COORDS="8,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm42.gif[/IMG] ';" COORDS="25,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm43.gif[/IMG] ';" COORDS="42,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm44.gif[/IMG] ';" COORDS="59,145,8">
<AREA SHAPE="circle" href="javascript:void(0);" onClick="document.REPLIER.EditedMessage.value+='[IMG]$NonCGIURL/smilies/cwm45.gif[/IMG] ';" COORDS="76,145,8">
<AREA SHAPE="rec" href="http://smilecwm.tripod.com/" Target="_blank" Coords="0,153,85,170">
<AREA SHAPE="default" NOHREF></MAP>);
}

----------
Find this:
----------

$SmiliesLink</font>

----------------
Replace it with:
----------------

$SmiliesLink</font><br>$SmileMapper

-----
DONE!
-----

Upload the postings.cgi file again and enjoy!

-SAL2000
