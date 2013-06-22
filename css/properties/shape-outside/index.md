{{Page_Title}}
{{Flags
|Content=Examples Needed
|Checked_Out=No
}}
{{Standardization_Status|W3C Working Draft}}
{{API_Name}}
{{Summary_Section|Wrap text around a given shape using floats.}}
{{CSS Property
|Initial value=auto
|Applies to=floats
|Inherited=No
|Media=visual
|Computed value=computed lengths for <basic-shape>, the absolute URI for <uri>, otherwise as specified
|Animatable=Yes
|CSS percentages=N/A
|Values={{CSS Property Value
|Data Type=auto
|Description=The float area uses the margin box as normal.
}}{{CSS Property Value
|Data Type=<basic-shape>
|Description=The shape is computed based on the values of one of ‘rectangle’, ‘inset-rectangle’, ‘circle’, ‘ellipse’ or ‘polygon’.

* <code>rectangle(&lt;x&gt;, &lt;y&gt;, &lt;width&gt;, &lt;height&gt; [, &lt;rx&gt;, &lt;ry&gt;])</code> defines a rectangle with an origin and a size. The optional arguments '''rx''' and '''ry''' define the "rounded corners" in the horizontal and vertical direction.
* <code>inset-rectangle(&lt;top&gt;, &lt;right&gt;, &lt;bottom&gt;, &lt;left&gt; [, &lt;rx&gt;, &lt;ry&gt;])</code> defines a rectangle by top, right, bottom and left insets. The optional arguments '''rx''' and '''ry''' define the "rounded corners" in the horizontal and vertical direction.
* <code>circle(<cx, <cy>, <r>)</code> defines a circle with a center point and a radius.
* <code>ellipse(<cx, <cy>, <rx>, <ry>)</code> defines a circle with a center point and a radii for the horizontal and vertical directions.
* <code>polygon(<x1> <y1>, <x2> <y2>, ..., <xn> <yn>)</code> defines a polygon based on a list of points
}}{{CSS Property Value
|Data Type=<uri>
|Description=If the <uri> references an image, which is CORS-same-origin, the shape is extracted and computed based on the alpha channel of the specified image. If the <uri> does not reference an image or if it references an image which is not CORS-same-origin, the effect is as if the value ‘auto’ had been specified.
}}
}}
{{Examples_Section
|Not_required=No
|Examples={{Single Example
|Description=This is a working example pulled from the Editor's Draft.
|LiveURL=http://code.webplatform.org/gist/5832982
}}{{Single Example
|Language=CSS
|Description=shape-outside using a rectangle equal to the content box
|Code=shape-outside: rectangle(0, 0, 100%, 100%);
}}{{Single Example
|Language=CSS
|Description=shape-outside using an inset rectangle 10px smaller than the content box in each dimension
|Code=shape-outside: inset-rectangle(5px, 5px, 5px, 5px);
}}{{Single Example
|Language=CSS
|Description=shape-outside using a rounded rectangle
|Code=shape-outside: rectangle(0 ,0, 100%, 100%, 10px, 10px);
}}{{Single Example
|Language=CSS
|Description=shape-outside using a circle filling the content box
|Code=shape-outside: circle(0, 0, 50%);
}}{{Single Example
|Language=CSS
|Description=shape-outside using a ellipse wider than it is tall
|Code=shape-outside: ellipse(0, 0, 50%, 30%);
}}{{Single Example
|Language=CSS
|Description=shape-outside using a diamond described as a polygon
|Code=shape-outside: polygon(50% 0, 100% 50%, 50% 100%, 0 50%);
}}{{Single Example
|Language=CSS
|Description=shape-outside using a shape from the alpha channel of an image
|Code=shape-outside: url(path/to/image.png);
}}
}}
{{Notes_Section}}
{{Related_Specifications_Section
|Specifications={{Related Specification
|Name=CSS Shapes Module Level 1
|URL=http://dev.w3.org/csswg/css-shapes/
|Status=Editor's Draft
}}{{Related Specification
|Name=CSS Shapes Module Level 1
|URL=http://www.w3.org/TR/css-shapes/
|Status=First Public Working Draft
}}
}}
{{Compatibility_Section
|Not_required=No
|Imported_tables=
|Desktop_rows=
|Mobile_rows=
|Notes_rows=
}}
{{See_Also_Section
|Manual_links=See also: [[css/properties/shape-margin|shape-margin]] property

See also: [[css/properties/shape-image-threshold|shape-image-threshold]] property
}}
{{Topics|CSS}}
{{External_Attribution
|Is_CC-BY-SA=No
|MDN_link=
|MSDN_link=
|HTML5Rocks_link=
}}