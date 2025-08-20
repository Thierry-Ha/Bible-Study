<%*
let title = tp.file.title
var TemplateText;
if(title.startsWith("%")) { 
	TemplateText = await tp.file.include("[[Template Podcast]]") ; 
} else if (title.startsWith("§")) { 
	TemplateText = await tp.file.include("[[Template Discussion]]") ; 
} else if (title.startsWith("{")) { 
	TemplateText = await tp.file.include("[[Template Book]]") ; 
} else if (title.startsWith("(")) { 
	TemplateText = await tp.file.include("[[Template Articles]]") ; 
} else if (title.startsWith("+")) { 
	TemplateText = await tp.file.include("[[Template Youtube]]") ; 
} else if (title.startsWith("=")) { 
	TemplateText = await tp.file.include("[[Template Ideas]]") ; 
} else if (tp.file.path(relative = true) == “20 Alignement/21 Values/test.md”  { 
	TemplateText = await tp.file.include("[[Test template]]") ; 
} else {
	TemplateText = await tp.file.include("[[Basic Note]]")
}; 
tR += TemplateText;
%>