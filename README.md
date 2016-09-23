# vnk (beta)
## .vnk / .vink file extension usage

This supports the use for inkVerb's .vink or .vnk filetype.
VNK is a local/cloud HTML document or markdown text file (depending on the file declaration inside) that can be used for
- rich text doc
- email
- blog post

Both .vnk and .vink file extensions work, much like .htm and .html. .vnk is typically generated locally as a local document while .vink is usually generated on a web server for email or blog posts. While this is typical and standard practice, it is not a requirement.

The HTML version will begin with the line:
<!DOCTYPE vink>
*This file would include the selective HTML tags used by the WordPress editor, without the html and body tags, only tags used in the body, and allowing the <vink /> self-closing XML tag and a <vink-email> tag.*
- <vink /> may include basic blogpost and document meta, such as publish status, author, etc.
- <vink-email> tag containing email header meta.
- The file may contain both <vink /> and <vink-email> tags.
- The <vink /> tag normally appears at the top while the <vink-email> tag normally goes at end of the document.

The text markdown version will begin with the line:
#!/vnk
*This filw would use basic Markdown notation.*
- Note that a special version of vnk markdown is planned to use post-word tags, such as ending& or ending$ or ending# or ending@ to make normal Markdown codes even shorter.
