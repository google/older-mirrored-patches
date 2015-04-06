In January 2006, Google contracted with [CodeWeavers](http://www.codeweavers.com/) to improve Wine to run Picasa version 2.2 properly. Some of the changes fix bugs in Wine; others implement previously unimplemented features. This effort resulted in 225 patches committed to winehq between 1 January and 18 April 2006. See the list below, or [download the exact Wine source tarball used for Picasa 2.2 (14 MB)](http://google-older-mirrored-patches.googlecode.com/files/picasa-wine-2.2.2820-5.tgz).

We also asked a few interns (Benjamin Arai, Dan Hipschman, James Hawkins, and Thomas Kho), to improve a few areas of wine (e.g. oleaut32, widl, msi, and riched20). Together they committed about 300 patches to the winehq git tree.

During 2007, we continued to improve Picasa, committing a few dozen patches to the winehq git tree. See the patches by Lei Zhang and Nigel Liang below.

We also contracted with Codeweavers to improve Wine so it could run Photoshop CS2 properly. As a result, about 200 patches were committed to winehq, and as of wine-0.9.54, [Photoshop CS2 is quite usable](http://wiki.winehq.org/AdobePhotoshop).

But wait, there's more! We also asked a few interns (Dan Hipschman, Evan Stade, James Hawkins, Jennifer Lai, Juan Lang, Mikołaj Zalewski, and Roy Shea) to improve a few areas of Wine (e.g. widl, gdiplus, msi, crypt32, and BITS), to get a few apps working better, and to scrape together a [win16 conformance test](http://win16test.googlecode.com/). During 2007, the interns committed about a thousand patches.

In 2008, we further improved support for Picasa and Photoshop, and fixed a few other bugs as well

Thanks again to Codeweavers and our interns (Maarten Lankhorst, Roy Shea, and Zac Brown) for a great job.

The following lists the patches described above, in reverse chronological order. (Note: although some care was taken in constructing this list, it may still contain some errors. Sorry if we've missed anything!)

| **Author** | **Date** | **Description** |
|:-----------|:---------|:----------------|
| Jacek Caban | 2008-10-06 | [jscript: Added possibility to run test scripts from file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68525652a15bcc332f1d48571bdb0f2da86bce47) |
| Jacek Caban | 2008-10-06 | [jscript: Fixed backslash handling in regular expressions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31b3071552b92fcd03988ee97764eb6249b80f57) |
| Jacek Caban | 2008-10-06 | [jscript: Don't initialize variables without initialiser to undefined in variable\_list\_eval. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=47b842bff7f93ac65b60230b506e4cf683c18817) |
| Jacek Caban | 2008-10-06 | [mshtml: Added IHTMLElement2::get\_currentStyle implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=56d1e9ec861e046c83b44203ea7d1e8ddcbac371) |
| Jacek Caban | 2008-10-06 | [mshtml: Added IHTMLStyle2 to IDispatchEx support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3203524bb5937750e287a4ed180d65592c7b40ed) |
| Jacek Caban | 2008-10-06 | [mshtml: Added IHTMStyle2 stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=239f7f70e77cdfe7466a6358d499fc5adb24d6ad) |
| Jacek Caban | 2008-10-06 | [mshtml.idl: Added IHTMLStyle2 interface declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cbeeac0ebfec70c816ef6e656f75bbe80d4b0d2d) |
| Dmitry Timoshkov | 2008-10-02 | [winex11.drv: Add support for \_NET\_WORKAREA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9aaa24091f9b93f8071b9685b6eaa8c6f16ff826) |
| Jacek Caban | 2008-10-01 | [jscript: Added delete expression for EXPRVAL\_IDREF implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c248189f7ac0770adca62df351e3e80c3a2de27) |
| Jacek Caban | 2008-10-01 | [jscript: Added IDispatchEx::GeleteMemberByDispID implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=65a207466dd3422e69e2dce302384414f23e67f0) |
| Jacek Caban | 2008-10-01 | [jscript: Added Date constructor object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84d8cddcae73b6a130fdae20636712ddb0f91c94) |
| Jacek Caban | 2008-10-01 | [jscript: Don't clear uninitialized variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a9c4d2b18e49957635fe0f942a1357cdf4cd59f7) |
| Jacek Caban | 2008-10-01 | [jscript: Allocate variables when entering execution context.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50a84b454541eba099b082d9fa912df538b1c4ab) |
| Jacek Caban | 2008-10-01 | [jscript: Optimize GetDispID usage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=131d0b9f1be05b51a9d54bd2fcc6999facf559ce) |
| Jacek Caban | 2008-10-01 | [mshtml: Ignore IDispatchJS in QueryInterface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b54f449e2d2514e3545d10e8e973339f8b55a2c6) |
| Jacek Caban | 2008-10-01 | [mshtml: Added IHTMLTableRow::get\_cells implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e80c55c367414f59961d1461e60760952d0bacc8) |
| Jacek Caban | 2008-10-01 | [mshtml: Added IHTMLTable::get\_rows implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac4117fdb5fc809aac2d23616d849563b2244bdf) |
| Jacek Caban | 2008-10-01 | [mshtml: Store nsIDOMHTMLTableElement in HTMLTable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf9155dbaa2760acde0239aca20ea76af8940c28) |
| Jacek Caban | 2008-10-01 | [mshtml: Use create\_all\_collection in IHTMLElement::get\_all implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0769ebc8a62db7f7e49e08c0f5d4650f3f645351) |
| Jacek Caban | 2008-10-01 | [mshtml: Use create\_collection\_from\_nodelist in IHTMLElement::get\_children implementation. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=53f00d02218d9d97908ef9a6faa9670768b18845) |
| Jacek Caban | 2008-10-01 | [mshtml: Move IHTMLElementCollection to separated file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c584effc737d5cc058f2cec6b54d456ae0e83ed3) |
| Jacek Caban | 2008-10-01 | [mshtml: Don't use IHTMLControlElement in IDispatchEx implementations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ee46d4814dabac5351d2f6a7fb85affdcdf7d2a) |
| Jacek Caban | 2008-10-01 | [mshtml: Added IDispatchEx support to IHTMLTable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=630252c12d3f7f54cf20f2685e41ddfc0f33bf48) |
| Jacek Caban | 2008-10-01 | [mshtml: Added IDispatchEx support to HTMLTableRow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea36413683f9ea7f64d6c0ce7ec181212e0e558d) |
| Jacek Caban | 2008-10-01 | [mshtml: Added IHTMLTableRow stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31ae80233ded69ad7ddee37b9070acbaad67776f) |
| Jacek Caban | 2008-09-30 | [mshtml.idl: Added DispHTMLTableRow declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b3c63dce6ee072122fefd6e65a3cc201aa64c1a) |
| Jacek Caban | 2008-09-30 | [mshtml.idl: Added DispHTMLTable declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7fb15065fc9b6b3438660304c9a657f74ae8bd7) |
| Jacek Caban | 2008-09-30 | [mshtml.idl: Added IHTMLTableRow declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d893690e3b45868eb89575f39a2a612e126f3592) |
| Alexandre Julliard | 2008-09-25 | [advapi32: Always pass a valid argv pointer to a service even if there are no arguments. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=cd3805336efd5d210474f6947f06d278985dff76) |
| Alexandre Julliard | 2008-09-25 | [gdiplus: Fix a string buffer overflow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a2d04673e6522036fe7f3d9ee3b7a10b6ae41435) |
| Jacek Caban | 2008-09-25 | [mshtml: Use ActiveScript for JavaScript in file protocol documents.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3bdda810243ed6c8d6b9960d1df3b534653b438) |
| Jacek Caban | 2008-09-25 | [jscript: Added String.split implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6906c2f1baf039dc7069d179a3e5d5c2f9e9b2c7) |
| Jacek Caban | 2008-09-25 | [jscript: Added String.match implementation for non-regexp arguments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9307a5ddfdb8fccdeabbd66f7e9a0fd9aa8258e3) |
| Jacek Caban | 2008-09-25 | [jscript: Added String.replace implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e0413ddfe598278df78519c5a79bd7689c045fd0) |
| Jacek Caban | 2008-09-25 | [jscript: Split regexp\_match function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b4796499e7bf6da2489eaf1c97c26a037053c494) |
| Jacek Caban | 2008-09-25 | [jscript: Added object to number conversion implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=136f7933c65bd5ef87de12083cf4a631ed07e58b) |
| Jacek Caban | 2008-09-25 | [jscript: Added Number default value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b3630ec7b75b329e255d29ce50a0a19b93ace1a) |
| Jacek Caban | 2008-09-25 | [jscript: Added VT\_R8 to string conversion implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53040deefd78575dfa1ce2bdc989038ce6b7a07d) |
| Jacek Caban | 2008-09-24 | [jscript: Fixed a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=87e2c255491a0b52ed2b13970448e5136f8f4c42) |
| Jacek Caban | 2008-09-24 | [jscript: Added RegExp contruction implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98f2dfee9cabde7fd62d11cd2850d608ec055aca) |
| Jacek Caban | 2008-09-22 | [jscript: Added Function default value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e806869d4e8b770ed63b94c22d703344f67e8ce2) |
| Jacek Caban | 2008-09-22 | [jscript: Added Function.toString implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5760eb808b17a8c80bbb42ea128499ace84b69af) |
| Jacek Caban | 2008-09-22 | [jscript: Don't call IDispatch as constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68bd72c7cd28bf1f1f80eb2f3d4f0091a2b74dda) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.ceil implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90dd23cc4c7416288ff8d5cb45523f073011f21e) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.pow implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4fe1b2efdb10c04a2a0fa984b42d7aa3e979880) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.max implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37b69e9a9eac535bc14ed8ee8afbc80954b00d12) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.abs implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2149494c9dfbfe7cf0d90090a6c2929cf8d79ef6) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.round implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c395981b2fef13008a4aa807869b7d657f38abd3) |
| Jacek Caban | 2008-09-22 | [jscript: Added Math.min implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50a24a4a1378e9bca1b6ff65055ab6d186048ee9) |
| Jacek Caban | 2008-09-22 | [jscript: Added String function implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=17ceb90b30f14fba20c8205870f2a2f89f7a1e6b) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.concat implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6751644835cc374baf5e04b80d878cee9f69c956) |
| Jacek Caban | 2008-09-22 | [jscript: Added String default value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f134b41b32dc92738fcbb1730e68c72845d7f06) |
| Jacek Caban | 2008-09-22 | [jscript: Added String constructor implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3925f13023161e9beda334a61b026ba78c58df4b) |
| Jacek Caban | 2008-09-22 | [jscript: Remove no longer used jsdisp\_set\_prototype.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84b69fb1aaa9b05402cdcfd9663f0fbfd2ebf760) |
| Jacek Caban | 2008-09-22 | [jscript: Added parseInt implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8537b6eb976ea65136d8ba0b0190c422974c5db) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.charCodeAt implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8612ae880f5db8d16192711f80565e7862f7e39e) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.slice implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2c6847d000655cc94ecb7bc729d6752748921af5) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.valueOf implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1388a6f421162736814d627c5d829405d72c8f46) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.toString implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=304e9fe0d41715b59468b58dad5f3e457565e764) |
| Jacek Caban | 2008-09-22 | [jscript: Added String.substring implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5fdf258b1a3e16a098d0d8e69d22185460d3c97f) |
| Jacek Caban | 2008-09-22 | [jscript: Fixed typo in to\_integer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dff4f0b598ba66d0f201488a67fd9291ead8344c) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array default value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=898cb6fcd43fc8038c74c45552b69ef29a19e0da) |
| Jacek Caban | 2008-09-22 | [jscript: for..in is not error if in expression is not an object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2efae9e79b1cf6f7a2980d40b8d54b323f801761) |
| Jacek Caban | 2008-09-22 | [jscript: Added Object default value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c6188fdffcb2e2b0c6129d8777499378999393b3) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array.concat implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5fa649cae6c95114ad7ecaaae216b4b9c8262be0) |
| Jacek Caban | 2008-09-22 | [jscript: Fixed array literal length calculation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=45cd5bc4a22926fe3a896992ae8606e4e8bc8e8d) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array.sort implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1f2e8e6c575922d28216fd9a7be42458a770c60) |
| Jacek Caban | 2008-09-22 | [jscript: Added Number function implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53e831e2cb62fda468bf63c02ece2d31de5428d2) |
| Jacek Caban | 2008-09-22 | [jscript: Added Number.toString implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3e2a6f9d7897d9615e35ebcc971723238d11376) |
| Jacek Caban | 2008-09-22 | [jscript: Added Number constructor implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b74d6a91cdd1d46e7543cb312f759ab586055bd) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array.toString implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b13719cd23f3e7bc29d4d3b6e0ffba2638ed835) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array.join implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f62dd2a9fdc2a768205f93177285e89173caa093) |
| Jacek Caban | 2008-09-22 | [jscript: Added Array.push implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=34e82951c3ebaa78fed3bd1d9315d1f605011973) |
| Jacek Caban | 2008-09-22 | [jscript: Added string to number conversion implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91b798ddf802bb9d7e812d84df308a324f555652) |
| Jacek Caban | 2008-09-22 | [mshtml: Fixed dynamic properties allocation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e9277986c85463f638328ffd7e64a48a21940427) |
| Jacek Caban | 2008-09-19 | [jscript: Added function constructor object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e07e0cf53357432002bd0804987cf102f677a72) |
| Jacek Caban | 2008-09-19 | [jscript: Added more to\_string implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4778c069039a567da9f86858da9fc3b3ea71b3a5) |
| Jacek Caban | 2008-09-19 | [jscript: Minor fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3435603520b8da0514b959c97e428904edffd294) |
| Jacek Caban | 2008-09-19 | [jscript: Added '>>>=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1b76a333b79ea94e3a7fc9108fcb8162263e8c4) |
| Jacek Caban | 2008-09-19 | [jscript: Added '>>=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc641097a90410c4a845d1ad17a3a82b561e13ec) |
| Jacek Caban | 2008-09-19 | [jscript: Added '&lt;&lt;=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=701797489d3b683a29af54ede839833caa0d6832) |
| Jacek Caban | 2008-09-19 | [jscript: Added '&gt;&gt;&gt;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=13790a640b463aa97caae8bbfd1e393d5c001f4d) |
| Jacek Caban | 2008-09-19 | [jscript: Added '&gt;&gt;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74fefe94ebe5d43c49a20fdcd4c4c092bcf16bc5) |
| Jacek Caban | 2008-09-19 | [jscript: Added '&lt;&lt;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef78010df4975ccdd98c0f7496327505f39026c3) |
| Jacek Caban | 2008-09-19 | [jscript: Added with statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfb867af56f4b15986482deef588d33d2458b101) |
| Jacek Caban | 2008-09-19 | [jscript: Added delete expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e9749bf921e8ec4cd40dcfb3447a9e85a5cd3ff) |
| Jacek Caban | 2008-09-19 | [jscript: Added for..in statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e162404674d6981248fe940fca332ef58b9a785) |
| Jacek Caban | 2008-09-19 | [jscript: Added String.charAt implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4731f174352033a2d2c226afdf94b334b5a4ef22) |
| Jacek Caban | 2008-09-19 | [jscript: Added void expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=536573934afb2722fc5867c39233a283f378c227) |
| Jacek Caban | 2008-09-18 | [jscript: Added for statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e68badeaf63cf514d32c3a22038adf87fa13258) |
| Jacek Caban | 2008-09-18 | [jscript: Added continue statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99335680630f0a48e999a2426b835dfb248e1459) |
| Jacek Caban | 2008-09-18 | [jscript: Added while and do..while statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7bde1a3345fb98075b0d5ed1d5cd16d159beb58a) |
| Jacek Caban | 2008-09-18 | [jscript: Added String.length implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b48489be3c884aecca8b5f3dd8f9eb21d4baa989) |
| Jacek Caban | 2008-09-18 | [jscript: Added to\_string(VT\_I4) implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1372814695510564f53645346c1eab8b1dc0d0c) |
| Jacek Caban | 2008-09-18 | [jscript: Added array literal implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=788197d592794849c981c79d8c6449f90bcec2b6) |
| Jacek Caban | 2008-09-18 | [jscript: Added eval implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44849c3fc90d09f18559d6f8e5ff190fc68efb0b) |
| Jacek Caban | 2008-09-18 | [jscript: Added bool and null to number conversion implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1bbc34f2f2c02b4e9087bd5f06c79804f6c94dfa) |
| Jacek Caban | 2008-09-18 | [jscript: Added plus expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c6b6c8ca840dc591d05bd3395163fb82eea7c3e) |
| Jacek Caban | 2008-09-18 | [jscript: Added '~' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=20bc98d5d86e6c0847a9be75b3272f4ba25d3712) |
| Jacek Caban | 2008-09-18 | [jscript: Added ',' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c0bfbba859c99d4680d51bac73d7dd1661ac4758) |
| Jacek Caban | 2008-09-18 | [jscript: Added '^=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5288c5b07c8f0116d298cb6cece49b26d10cbf6c) |
| Jacek Caban | 2008-09-18 | [jscript: Added '^' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7202197dfa0654a515dc85ebd0e77bad78b5c8a7) |
| Jacek Caban | 2008-09-18 | [jscript: Added '&=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8aeb15cb58f6ea5066dc847c11c62a8f52bd1a7) |
| Jacek Caban | 2008-09-18 | [jscript: Added '&' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d2de1d310375d0fa97ff7f5b0b0cb93e1eca8d6b) |
| Jacek Caban | 2008-09-18 | [jscript: Added '|=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a51ec811c727c62defde5942861d5ea58749cd6b) |
| Jacek Caban | 2008-09-18 | [jscript: Added '|' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ec6411a7fca04c41b843f4776a481d712bd4952b) |
| Jacek Caban | 2008-09-18 | [jscript: Added break statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32a3a167b6d133f6836a3fc264b0251c315ac783) |
| Jacek Caban | 2008-09-18 | [jscript: Added switch statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b16387708b2fc1842f726b899e8584eaf5c639f) |
| Jacek Caban | 2008-09-18 | [jscript: Added 'new' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c0f3c78954e1e7f65644fba97cfc52c60f9b5cf4) |
| Jacek Caban | 2008-09-18 | [jscript: Added '!=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47fcf8d0c7359865a99c10d5d1843580e8cc4d19) |
| Jacek Caban | 2008-09-18 | [jscript: Added '==' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d699834892c0a47362c2f004a3222713ebda39ba) |
| Jacek Caban | 2008-09-17 | [mshtml: Fixed tests on IE7.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef221478f02a18fa867dd2fa07e87fcfd90054eb) |
| Jacek Caban | 2008-09-17 | [jscript: Fixed allocation of script buffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e670c1c6bde92bb6d760f7e3aca9850f2862492) |
| Lei Zhang | 2008-09-17 | [qcap: Make sure input to AMStreamConfig\_SetFormat is not NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62823d272dd988f9417fa1bc4207c8cc9467d7d0) |
| Jacek Caban | 2008-09-16 | [jscript: Added minus expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c1c923d5efd86a03bbddb9e574dc90727485691) |
| Jacek Caban | 2008-09-16 | [jscript: Added '/=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43f760ba1751430aa4543c94d1b259d9bdfd577a) |
| Jacek Caban | 2008-09-16 | [jscript: Added '/' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=323e11b4abb0bfa8f347da1789f233e52ca6ed13) |
| Jacek Caban | 2008-09-16 | [jscript: Added '\*=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01a4acbd8c377bebd03c9767a4bc3aa5d3c081b0) |
| Jacek Caban | 2008-09-16 | [jscript: Added '\*' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2385f8d494ca7a848309760381f321d04b83ebd1) |
| Jacek Caban | 2008-09-16 | [jscript: Added '-=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a672e334e1655e400beb9eca1179dc49cd417f3) |
| Jacek Caban | 2008-09-16 | [jscript: Added '-' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3af87180a7cd6f9ffeff848737a1abed69b47ed) |
| Jacek Caban | 2008-09-16 | [jscript: Added to\_object(number) implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a97632a4e1a5f653fbfacb695b6c2b6bf9af73f) |
| Jacek Caban | 2008-09-16 | [jscript: Added to\_object(VT\_BOOL) implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7fa373e364320369eed110f51baad7639be4a8e0) |
| Jacek Caban | 2008-09-16 | [jscript: Added throw statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7903ecfa9aaa07ecf6ad32ffc5a15eb9cf73353) |
| Jacek Caban | 2008-09-16 | [jscript: Added try statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=66eb62ada690914070a7ee275a8ce253eef84a62) |
| Hans Leidekker | 2008-09-16 | [winhttp: Fix logic inversion bug in setting disable flags.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d943ffa6f798f106bc7e4b398bab9622f97a85b7) |
| Hans Leidekker | 2008-09-16 | [winhttp: Manage a session global cookie cache.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a706aae706a1636555e5528b0ad91936fc3e69c) |
| Hans Leidekker | 2008-09-16 | [winhttp: Move handling of default request parameters back to WinHttpOpenRequest.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ae5741c4e8a9ec7568a9e46da65ea1a44e1d643) |
| Hans Leidekker | 2008-09-16 | [winhttp: Reset content length when all data has been read.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8df906f28e9f1bd53bc105f5b4a0d06adaca2ac2) |
| Jacek Caban | 2008-09-16 | [jscript: Added RegExp tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b9bc9816b268f855fa25524f0b20a94062385b0) |
| Jacek Caban | 2008-09-16 | [jscript: Added String.match implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db69b121ac6e3306d95911c00b18fc1c7c4f5b67) |
| Jacek Caban | 2008-09-16 | [jscript: Added string to object conversion implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a752be1a799563e0790d2203917434c6d5ecea1) |
| Jacek Caban | 2008-09-16 | [jscript: Added regular expression  compiler based on Mozilla regexp implementation. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=5670ca52ae50eba30775b20e65b48e6de39db5cb) |
| Jacek Caban | 2008-09-16 | [jscript: Reuse temporary heap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ac24dc2bf9dc6cf783405968162461867a36aeb) |
| Jacek Caban | 2008-09-16 | [jscript: Added parser support for regular expressions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf1863ed09d2e2930b873f75c9aa696883a48237) |
| Jacek Caban | 2008-09-16 | [jscript: Added ArrayInstance::on\_put implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2e7626c7a24c1c927b9469fa29cef55689ef894) |
| Jacek Caban | 2008-09-16 | [jscript: Added Array.length implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06d19171be21fde7bff7b7551c1b56baba301cdb) |
| Jacek Caban | 2008-09-16 | [jscript: Added Array constructor implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c25917e5d94fd89a192d23a42032ce3d0354be5) |
| Jacek Caban | 2008-09-16 | [jscript: Added missing RegExp properties.](http://source.winehq.org/git/wine.git?a=commitdiff;h=199952bf5590d1acff24445d6f9479aa8aa8b432) |
| Roy Shea | 2008-09-15 | [kernel32/test: Test import entries of a core windows DLL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91e33020f05618826a378b540a234f400a660ac8) |
| Alexandre Julliard | 2008-09-12 | [winex11: Driver-side implementation of SetLayeredWindowAttributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be3c3a52141e100075c11896ac96e50736411ae3) |
| Alexandre Julliard | 2008-09-12 | [user32: Add a SetLayeredWindowAttributes driver entry point.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9fb76ddd53fef4dc6b1e4a01c8f39aac326e4e22) |
| Alexandre Julliard | 2008-09-12 | [user32/tests: Added some tests for Get/SetLayeredWindowAttributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d476761f912a3f217e6356119cf328cfad4de3e2) |
| Alexandre Julliard | 2008-09-12 | [server: Implemented the server side of Get/SetLayeredWindowAttributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05b4181cac1f567f786a0ce7c182adb7e7355880) |
| Alexandre Julliard | 2008-09-12 | [user32: Notify the user driver about window extended style changes too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f1121316868b79bfe01105b6a3814a17ec655d5) |
| Jacek Caban | 2008-09-12 | [mshtml: Added body dispatch id test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1c51d3598df31a196320c74fb39f9fa33f537dc9) |
| Jacek Caban | 2008-09-12 | [jscript: Added postfix decrement expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2950c3fa2d9726af00adedd05083d58b11e67ee0) |
| Jacek Caban | 2008-09-12 | [jscript: Added postfix increment expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b291b83a6bfb3fbfb988048270e9c188acefefd8) |
| Jacek Caban | 2008-09-12 | [jscript: Added prefix decrement expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce423c2e3bdf0ba1d8d5c8f6ad7191bfbf07c173) |
| Jacek Caban | 2008-09-12 | [jscript: Added prefix increment expression.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5df7ac456f0a812fe8d20d249061ab0101afd746) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&gt;=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa4f801ed0abdca2c8256645bb8c92dbd0a8d70f) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&gt;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa0c254e4afc57ce93ba4026dc8efa70f00b4b85) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&lt;=' implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9332be04f0f07a3f8a6be71273ec0973ffd60da0) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&lt;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e2a9ae06a92b7602f184160103bdeaff8104993) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&&' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc9e6aa1e5a0124b14a832d75f0c7ead998d4f1d) |
| Jacek Caban | 2008-09-12 | [jscript: Added '&#124;&#124;' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d541ecc5dff7cb6a07d8b1a0ab488a1b68a82d2) |
| Jacek Caban | 2008-09-12 | [jscript: Added '+=' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50c7c4b7193cf21a956d2bdba656dc09e6f5fb26) |
| Hans Leidekker | 2008-09-11 | [winhttp: Strip content-type/length headers from request on a redirect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=10090eb2527ec86eec6c011b1d7c7f2318ea0c55) |
| Hans Leidekker | 2008-09-11 | [winhttp: Preserve cookies on redirects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bddcb1b8bbb13e9ca87cb28f78f06f06c83f69b6) |
| Hans Leidekker | 2008-09-11 | [winhttp: Redirects are always GET requests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0451643e02b97480c3d0a23a3b05ac46159d553c) |
| Hans Leidekker | 2008-09-11 | [winhttp: Handle relative redirects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=28ae1d4f0dc55c59532c33a3d3d3443f23195c05) |
| Jacek Caban | 2008-09-11 | [jscript: Added add expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=93a62e8f70be1eeb208799ea0217f97823baa250) |
| Jacek Caban | 2008-09-11 | [jscript: Added script types tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=beba0f711d0059b186dd205b0fcd09c253eac4c3) |
| Jacek Caban | 2008-09-11 | [jscript: Added conditional expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23ccc9a293c6261e035a29f211970bf7c4a37fc5) |
| Jacek Caban | 2008-09-11 | [jscript: Added block statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=026bbea6726ad396500bc45f380e3cb18ed506e5) |
| Jacek Caban | 2008-09-11 | [jscript: Added object initialiser expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7786d1d4588934d3ba9ccf1f457adfa1c16d89d) |
| Jacek Caban | 2008-09-11 | [jscript: Added if statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1edd64ef8b453ed44ab3f234d8b3d7be6d62e389) |
| Jacek Caban | 2008-09-11 | [jscript: Added IActiveScriptParseProcedure2::ParseProcedureText implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eedc6dc715096488be5576c987860e6ad8986164) |
| Jacek Caban | 2008-09-11 | [jscript: Release named items in IActiveScript::Close.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44333104ced7668f10345f4053a2f1d62a0cf43d) |
| Jacek Caban | 2008-09-11 | [jscript: Added initial prototype of functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0c6b804e6302a05cd29cead8df12af6ca2f954fd) |
| Jacek Caban | 2008-09-11 | [jscript: Added function expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2a93fe3c3f3bf820744cbeb21b8ea5c31d8608f) |
| Jacek Caban | 2008-09-11 | [jscript: Added constructor invokation from Function object support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4e47c01498ae4c1d4e96da5ede061e2b7bc2000) |
| Jacek Caban | 2008-09-11 | [jscript: Added Object constructor implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bea575c9163465db5a7df8da8580e9d4443cec01) |
| Jacek Caban | 2008-09-11 | [jscript: Added 'new' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=152b3e48c119f2bfe8325471ecca8ca52ca1d8ea) |
| Jacek Caban | 2008-09-11 | [jscript: Added array expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ef7038ba512a337c85b10bb981c3cf8b958d2b7) |
| Jacek Caban | 2008-09-11 | [jscript: Set arguments object on function call.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68d4f489f2d26bddef00eae71608e40fb2c4ab22) |
| Jacek Caban | 2008-09-11 | [jscript: Set parameters on function call.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0d33508954880b31f8b70b24ebb229195fdd05db) |
| Jacek Caban | 2008-09-11 | [jscript: Added Function.[[call[](http://source.winehq.org/git/wine.git?a=commitdiff;h=dd9f8f7dbc7a9010a610dee25567cee384d57cfd)][.md](.md)] implementation.] |
| Jacek Caban | 2008-09-11 | [jscript: Added return statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a273e35f9bd00b01c970c426d7614e3c0a80b229) |
| Jacek Caban | 2008-09-11 | [jscript: Added this expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0bd508db2f7e05d0317d3ab0e8eeb81219aa5572) |
| Alexandre Julliard | 2008-09-11 | [kernel32: Added implementation for UnregisterWaitEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee375f7c22f727c4a26e194c4076f3663d04d171) |
| Dmitry Timoshkov | 2008-09-11 | [user32: Fix the work area test to pass on Windows when the taskbar is on top.](http://source.winehq.org/git/wine.git?a=commitdiff;h=077cd6a9f5ecded0681098d6d89026a98983fe23) |
| Dmitry Timoshkov | 2008-09-11 | [user32: Implement SystemParametersInfo(SPI\_GETWORKAREA) properly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c707e7d9a6a5c804b3ae286c9bd8bab279327dc6) |
| Dmitry Timoshkov | 2008-09-11 | [user32: Make GetMonitorInfoW print the monitor properties.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5587387c9f07e0632d81090a1364b749156c90fd) |
| Lei Zhang | 2008-09-11 | [comctl32: Handle listview dragging better.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc2404bc206b07f7ffe6e980a026d1badf9d1376) |
| Lei Zhang | 2008-09-11 | [comctl32: listview: Prevent DragDetect from removing WM\_LBUTTONUP messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5f9b0db21798e863c234fdc287fa3cfaa8a3cfe1) |
| Roy Shea | 2008-09-11 | [shell32: Use default system icons if PrivateExtractIconsW in SHGetFileInfoW...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b6806922aedc00e445f009389b2832c5da690ac) |
| Jacek Caban | 2008-09-10 | [jscript: Added typeof expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=67684c48509458d6b8d669333e2fe13febc6a196) |
| Jacek Caban | 2008-09-10 | [jscript: Added Math object stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=083c95449ec28435a3888f7b99b28b4126e6a96f) |
| Jacek Caban | 2008-09-10 | [jscript: Added RegExp constructor object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e2f743fad8b8ddc0ac3073f33d92855e1abee2fe) |
| Jacek Caban | 2008-09-10 | [jscript: Added Number constructor object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a3d60e9130aca54b0561c5cadc0468c27fd38d8) |
| Jacek Caban | 2008-09-10 | [jscript: Added Boolean constructor object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8be53fcf33208861887351be6f97861b1133763) |
| Jacek Caban | 2008-09-10 | [jscript: Added Array constructor object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54d03ab8579cd7d1d5255b2e7b6a6a4405f8e66c) |
| Jacek Caban | 2008-09-10 | [jscript: Added String constructor object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8482abe29ccdd2f39f6918c5dc8272a4d0de832e) |
| Jacek Caban | 2008-09-10 | [jscript: Added Object constructor object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dd01f8b8f79d46e0fa951f5ab48b309ff744f581) |
| Hans Leidekker | 2008-09-10 | [winhttp: Better diagnostics in the notification test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3cfa9c626f92f24f0f7e893bb5c079571fc493ee) |
| Hans Leidekker | 2008-09-10 | [winhttp: Increase sleep between two tests that connect to the same host.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ddbe713e6bdfedd0da03523f91ee3ecde59ad8ef) |
| Hans Leidekker | 2008-09-10 | [winhttp: Don't loop on response codes other than 301 and 302.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8f9c4cb9cc45075b829e3ffbdeb88a6c00c0ece) |
| Alexandre Julliard | 2008-09-09 | [user32: Fix DeferWindowPos to work on windows belonging to other processes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3f4fb4929284085b8d634f932299e672eaa692e) |
| Jacek Caban | 2008-09-09 | [jscript: Added '!==' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7c8c2544d82d550459ff28cad2b1b64cf39227b) |
| Jacek Caban | 2008-09-09 | [jscript: Added Function.length implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0170ad7f9719ad60a8c80629b9a1e8f982ea95c) |
| Jacek Caban | 2008-09-09 | [jscript: Added member expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99b4bc2347b4eac6103cc73880188d6463cb4aab) |
| Jacek Caban | 2008-09-09 | [jscript: Added function object stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c6bf428b5a7883de2ed0813f746e5c3704e2683) |
| Jacek Caban | 2008-09-09 | [jscript: Add static functions to variable objects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c05e6c8692c930525d2f61c01228a579b4b4e03) |
| Jacek Caban | 2008-09-09 | [jscript: Added scope chain implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc5a8836e9e41c97536c372bf4c5c945701f21be) |
| Jacek Caban | 2008-09-09 | [jscript: Added global object implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca2b797f6a7e5fa2f320fed0c4aaab70c0d44068) |
| Jacek Caban | 2008-09-09 | [jscript: Added '===' expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3938073dad90bcbd762768b2731bb8fa11b5456) |
| Jacek Caban | 2008-09-09 | [jscript: Added infrastructure for test scripts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b60898353c47a507f08ccbf45748922adde93afb) |
| Jacek Caban | 2008-09-09 | [jscript: Added call expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a16f205382994d39a0a10cafac9857a3682321d3) |
| Jacek Caban | 2008-09-09 | [jscript: Added assignment test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=86a787bbc9a62bbd3d192ae953848bc7201864f1) |
| Jacek Caban | 2008-09-09 | [jscript: Added variable object handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=652a0121a9cf55d47bce176bcbb7e55c6927ec04) |
| Jacek Caban | 2008-09-09 | [jscript: Added assign expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=512505f9085781521c2e6693dde5e3d4bfbfee0d) |
| Jacek Caban | 2008-09-09 | [jscript: Added literal expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c05ffe09487b66da4d377aaf0e76f24bd45449c) |
| Jacek Caban | 2008-09-09 | [jscript: Added var statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=326cf6e0cf39203571ccfa33373184c79c17dc9f) |
| Jacek Caban | 2008-09-09 | [jscript: Added AddNamedItem implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2bbd9d410509a426b22f59c156daa15a35b78809) |
| Jacek Caban | 2008-09-09 | [jscript: Added identifier expression implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a7c9f1b922218ed1505d77812f8e1187efec81f) |
| Jacek Caban | 2008-09-09 | [jscript: Added logical negation implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11153d0e0542d623d25dc46a14dfff846efbb867) |
| Jacek Caban | 2008-09-09 | [jscript: Added expression statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb0bb55de28c5aa3183a3696d8e2823f0828de94) |
| Jacek Caban | 2008-09-09 | [jscript: Added DeleteMemberByName implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68326a391de3f22f13048f6c973398340825800f) |
| Jacek Caban | 2008-09-09 | [jscript: Added InvokeEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=61734cd94517f05a179e9ec639e6e8d363eb91cf) |
| Jacek Caban | 2008-09-09 | [jscript: Added GetMemberName implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3612bae30c0496d13d076358ab41478e337deee6) |
| Jacek Caban | 2008-09-09 | [jscript: Added GetNextDispID implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11d9a49b0a58cef37badf9e65fb8b3b0197a1317) |
| Hans Leidekker | 2008-09-09 | [winhttp: Make sure not to read more data than expected on a redirect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f28c5f87e23fe4a079d1f1fb184228212a39709) |
| Hans Leidekker | 2008-09-09 | [winhttp: WinHttpQueryDataAvailable should do a blocking read if more data is expected. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=01e7d128483cf4bec401dee3fc8a479109d7a072) |
| Hans Leidekker | 2008-09-09 | [winhttp: Option WINHTTP\_OPTION\_SERVER\_CERT\_CONTEXT must return a pointer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e6ffab63f1a44da02c817074c2cf009bfdd6a84) |
| Alexandre Julliard | 2008-09-08 | [winex11: Support setting the window region on windows belonging to other threads. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d45cfde33f49339956167206a10da7229608df6) |
| Alexandre Julliard | 2008-09-08 | [winex11: Moved the X11DRV\_WindowMessage function to window.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=370368aace67b0bad2ce7813e800f668eaa8c027) |
| Jacek Caban | 2008-09-08 | [jscript: Store more data in DispatchEx object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c23ea508a1af4f4f64ae9b33f43c2c44ac00b698) |
| Jacek Caban | 2008-09-08 | [jscript: Added GetDispID implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ac404aa9c8e3279f6ad8ef6126196e54ad5a2b1) |
| Hans Leidekker | 2008-09-08 | [winhttp: Support asynchronous requests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f3346a789ea01e578b93c7d4f0fdf870f80b446d) |
| Hans Leidekker | 2008-09-08 | [winhttp: Add the remaining completion notifications.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4d0abb2344f93552add6eef9a723573c76ba6a2) |
| Hans Leidekker | 2008-09-08 | [winhttp: Implement WINHTTP\_OPTION\_SERVER\_CERT\_CONTEXT.](http://source.winehq.org/git/wine.git?a=commitdiff;h=64a7d23565640b3815676cd53eba169fc246cccf) |
| Hans Leidekker | 2008-09-08 | [winhttp: The last parameter of WinHttpWriteData is optional.](http://source.winehq.org/git/wine.git?a=commitdiff;h=520b6e815397b91c13b3ff135a503577532df226) |
| Hans Leidekker | 2008-09-08 | [winhttp: Start sending async completion notifications. Add corresponding tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d8a9564cde87f34d9404917e0265b7d0fa8bdb7) |
| Hans Leidekker | 2008-09-08 | [winhttp: Use a process global SSL context instead of per connection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2fb746783f363b8a34f87476c997ba55ccb1c90f) |
| Lei Zhang | 2008-09-08 | [sane.ds: Replace wsprintfW with sprintfW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=887aa9eb3dd3fc22d4f50df125080f5fc82b583c) |
| Hans Leidekker | 2008-09-05 | [winhttp: The last parameter of WinHttpQueryDataAvailable and WinHttpReadData is optional. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ecd01b8d1f19c32d5acd09da51e4b10fde8197f) |
| Hans Leidekker | 2008-09-05 | [winhttp: Implement WinHttpQueryHeaders(WINHTTP\_QUERY\_RAW\_HEADERS).](http://source.winehq.org/git/wine.git?a=commitdiff;h=6fe2edb5def17acd18f420664eebffeac66ae8e5) |
| Hans Leidekker | 2008-09-05 | [winhttp: Implement WinHttpQueryOption(WINHTTP\_OPTION\_SECURITY\_FLAGS).](http://source.winehq.org/git/wine.git?a=commitdiff;h=b34e816f4a8a7284a29d1a20e56a5d37b63b897b) |
| Jacek Caban | 2008-09-05 | [jscript: Added empty statement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b40b352c8f8e995d06f1ab04742edadfc832cb05) |
| Jacek Caban | 2008-09-05 | [jscript: Added ParseScriptText test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a7ede8f272a4545a56703acbe97a52c7afd34553) |
| Jacek Caban | 2008-09-05 | [jscript: Added SCRIPTSTATE\_STARTED implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51a2ccb4c475295741c03efe98b8a46bb82c509b) |
| Jacek Caban | 2008-09-05 | [jscript: Added IActiveScript::ParseScriptText implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69f8b4b9b23013e8bf879cced575c910f10fdb09) |
| Alexandre Julliard | 2008-09-04 | [kernel32: Implemented the wrapper functions for job objects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b44a109b8c06ef2cf6b071dc7b00b742e2ce8001) |
| Alexandre Julliard | 2008-09-04 | [ntdll: Add stubs for all the job object functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=091d9748e3bc4494a2f1f6ee37a699fe98f875d4) |
| Alexandre Julliard | 2008-09-04 | [ntdll: Implemented NtOpenProcessTokenEx and NtOpenThreadTokenEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0327f84a2f9e70b416146ee97fdccb1827fe38b4) |
| Alexandre Julliard | 2008-09-04 | [winebuild: Generate MS-style imports using the OriginalFirstThunk field.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1abf80909981c9424b8bcc47ea363d02f585bf4f) |
| Alexandre Julliard | 2008-09-04 | [libwine: Add support for relocating MS-style imports that use OriginalFirstThunk. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=4eb350b86b50edf84a5587f54483c22ecb5a2750) |
| Jacek Caban | 2008-09-04 | [jscript: Added parser memory managment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=720e8c625225a91109c77ce11c34e4e2dc3977be) |
| Jacek Caban | 2008-09-04 | [jscript: Added lexer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b51a156ff1571d8c0af9e87b92d7949d82ecd0db) |
| Jacek Caban | 2008-09-04 | [jscript: Added parser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ebdd111264cfa646dd5219b5874166eb59217c1) |
| Hans Leidekker | 2008-09-04 | [winhttp: Implement some more options.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e078f618eb7c05c3cbec915f69a1d69fd3b35bed) |
| Hans Leidekker | 2008-09-03 | [winhttp: Add an initial implementation of WinHttpQueryOption and WinHttpSetOption. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=a74b52cf38402b4dc082e19eea880f7afd83881b) |
| Hans Leidekker | 2008-09-03 | [winhttp: WinHttpCrackUrl and InternetCrackUrlW use different scheme constants.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9f8d4fe082349a9079a666d7be0a2c2fd208b233) |
| Hans Leidekker | 2008-09-03 | [winhttp: Add status notification tests. Make them pass.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96bf72f27e3244e6fcad4677ca749e9e370f412c) |
| Hans Leidekker | 2008-09-03 | [winhttp: Move handling of default request parameters into build\_request\_string(). LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=8063f5cbd4332b8d66d4adc2a390f76d1875fd7c) |
| Hans Leidekker | 2008-09-03 | [winhttp: A non-standard port must be included in the host header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6bb3090732ef5a4dd4584e22738d0df418e5a8f2) |
| Hans Leidekker | 2008-09-03 | [winhttp: Avoid testing errno when it isn't set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=567e21e13255f24cf6318024c93be94180ad7b2b) |
| Hans Leidekker | 2008-09-03 | [winhttp: Handle redirects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41a763629f3150e5bcdf878e7d08554c50ef0f89) |
| Hans Leidekker | 2008-09-03 | [winhttp: Allow reusing a secure connection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=20d06b2a4cade847d8f4f7c252b5f6e1762dbb2a) |
| Hans Leidekker | 2008-09-03 | [winhttp: Add zero value content length header to POST requests without additional data. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=04a11bb11718337bd398658330d9e1529ff4b34f) |
| Dan Hipschman | 2008-09-02 | [oleaut32: Add a widl-generated proxy file for ocidl.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e6784c2a7dfa6d409069f513c870f253a31ab6e) |
| Dan Hipschman | 2008-09-02 | [widl: Output NULL for inherited methods in the vtbl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a41de877daa3936590d6db5f1456cfd4e7b55cec) |
| Dan Hipschman | 2008-09-02 | [ole32: Add a widl-generated proxy file for oleidl.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19cccae29d736e1328417ccc7d9d8f58b5eae293) |
| Dan Hipschman | 2008-09-02 | [ole32: Add a widl-generated proxy file for objidl.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44800b6ad4570b0f0b47c696d7e129523b6ce468) |
| Dan Hipschman | 2008-09-02 | [ole32: Add widl-generated proxies for unknwn.idl and dcom.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4afc326638201375438ed56b714453bc73421824) |
| Hans Leidekker | 2008-08-29 | [winhttp: Use default values when empty strings are passed for verb, object and version parameters. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=13ba609b0488fa28fc03bcde1262e62a6eae2178) |
| Hans Leidekker | 2008-08-29 | [winhttp: Test secure connections. Fix a crash when no response is returned.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f732065c4c8b8065701f49d8742a8d1a299205e7) |
| Hans Leidekker | 2008-08-29 | [winhttp: Add support for secure connections.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b19e8559f89f2b6a503821d2ac5fffb31aec6ac) |
| Lei Zhang | 2008-08-28 | [wininet: Remove redundant CrLf variables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f7e56d19c45f5b87bade0c4ecca3aa24d0264360) |
| Lei Zhang | 2008-08-28 | [wininet: Work around NULL headers when handling HTTP\_QUERY\_RAW\_HEADERS\_CRLF.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc9e214f6fb2ea68c9fcd7f635c47f3e85fc695c) |
| Lei Zhang | 2008-08-28 | [regedit: Fix typo in commit c6d01ac847edc2ad02ef02c7a0ead7a833539c3c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=faf9c55eb8fe296b508476a20f1899ce4c645409) |
| Hans Leidekker | 2008-08-27 | [winhttp: Implement WinHttpSetCredentials.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70c6a8ac62ecaf95a5c62ef154fef536b42715b2) |
| Hans Leidekker | 2008-08-27 | [winhttp: Implement WinHttpQueryAuthSchemes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f85f4552bf9ed54aa80fe61191083bab8c2598b) |
| Dmitry Timoshkov | 2008-08-27 | [user32: Add a test for monitor work area, fix some failures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dddec81dfbe13b202adbc36e59e6b92e0fe449f8) |
| Hans Leidekker | 2008-08-26 | [winhttp: Remove some unneeded includes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=18677beb571c641bc36d117ad550435b1c86c54e) |
| Hans Leidekker | 2008-08-26 | [winhttp: Implement WinHttpSendRequest.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f07f2304b0b30e2efac70f0a4defc0999a7b583e) |
| Hans Leidekker | 2008-08-26 | [winhttp: Implement WinHttpQueryDataAvailable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7f54676526454bfe2eefe0d26f66f6a292f71d9) |
| Hans Leidekker | 2008-08-26 | [winhttp: Implement WinHttpReceiveResponse.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b170ac20dd615e93c8831757d67e80b91f430abd) |
| Hans Leidekker | 2008-08-26 | [winhttp: Add support for querying most of the standard header attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac95d77e1f0980cbe0025012c5a06156ea910447) |
| Hans Leidekker | 2008-08-26 | [winhttp: Implement WinHttpReadData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=728bf77c83e331d821272131aaf8eb71600c2a77) |
| Hans Leidekker | 2008-08-26 | [winhttp: Implement WinHttpWriteData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6619e54d1eaf5f62115e8fa43a2db16589e47c16) |
| Hans Leidekker | 2008-08-26 | [winhttp: Add networking infrastructure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=266c4b2c046b334ca44cdc1826c4434625dcb29f) |
| Jacek Caban | 2008-08-26 | [jscript: Added JSGlobal typelib.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d367d9260f0e07ec3321abd5ac069edfd9d7c63) |
| Roy Shea | 2008-08-26 | [mstask: Implemented CreateTrigger.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c5f411e7ae82dd1ff6569adbb2c4f9a76a58103) |
| Roy Shea | 2008-08-26 | [mstask: Implemented (Set|Get)Trigger.](http://source.winehq.org/git/wine.git?a=commitdiff;h=65d987146390f0c69e86743cb5c8f214e967087b) |
| Jacek Caban | 2008-08-25 | [mshtml: Added IHTMLElement::get\_parentElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad156168d170c5119c1e62c398a91dcf84c0516a) |
| Roy Shea | 2008-08-25 | [mstask: Implemented PersistFile\_Save stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2172120fae14d1c69e8b2e6b9588acf6f00a6996) |
| Roy Shea | 2008-08-22 | [mstask: Implemented partial stub for (Set|Get)AccountInformation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f208025228852d2286ffcd8de7ba880216413d16) |
| Roy Shea | 2008-08-22 | [mstask: Task PersistFile AddRef, QueryInterface, and Release.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aec0eb87de7d71ab4d3160f3b2b0fb1250937243) |
| Roy Shea | 2008-08-22 | [mstask: Implemented (Set|Get)MaxRunTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a597d9eaed00489ba44cfb0ab339e7b60bd230ba) |
| Roy Shea | 2008-08-22 | [mstask: Implemented (Set|Get)Comment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37708b1e5c9923817384f5d51b9bd5e887d956a9) |
| Roy Shea | 2008-08-22 | [mstask: Implement (Set|Get)Parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f95e5123be7b967d261a75a69ca27f7cfe03970) |
| Maarten Lankhorst | 2008-08-22 | [dsound: Tune some parameters to make pulseaudio work.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc224421416bd2616bfd52431388a6f9630bc860) |
| Maarten Lankhorst | 2008-08-22 | [winealsa.drv: Tune some parameters to make pulseaudio work.](http://source.winehq.org/git/wine.git?a=commitdiff;h=944cb7ea15a3e8cbdded643b91ba85acbac827c8) |
| Lei Zhang | 2008-08-21 | [comctl32: Set listview focus on WM\_LBUTTONUP instead of WM\_LBUTTONDOWN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=098dc7b3302f39c5500d644615a6f4c37d328ce0) |
| Roy Shea | 2008-08-21 | [expand: Extended expand program to accept /r argument.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44941a55fa97b40b4c9ffa8e414e3a8a26efc65b) |
| Roy Shea | 2008-08-21 | [mstask: Implemented (Set|Get)ApplicationName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca736551240f510cba58770c0ec9e156904160e7) |
| Roy Shea | 2008-08-21 | [mstask/tests: Conformance test for (Set|Get)Trigger.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5536ef1ae494e2283e977ba702f863923900f15) |
| Roy Shea | 2008-08-21 | [mstask: TaskTrigger stub with AddRef, QueryInterface, and Release.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c131bb05691cf4fbbe76c4657099b13670478e1) |
| Roy Shea | 2008-08-21 | [mstask/tests: Basic conformance test for (Set|Get)AccountInformation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8d22f02df9882e673e3cd72f1ef4218a6fb22ef) |
| Roy Shea | 2008-08-21 | [mstask/tests: Conformance test for (Set|Get)MaxRunTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=714c6d3a66f0f31829ef95e84800d2d275a6e5e5) |
| Roy Shea | 2008-08-21 | [mstask/tests: Conformance test for (Set|Get)Comment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7cca21426adbc0fda58adff763d5fc5409283a1a) |
| Roy Shea | 2008-08-21 | [mstask/tests: Conformance test for (Set|Get)Parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cd8ac273046614430cf6d4359886442b7acd4bb0) |
| Hans Leidekker | 2008-08-20 | [winhttp: Add some tests for WinHttpAddRequestHeaders.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6603ad725a4f6f504f49cd587bc408268aa9d61f) |
| Hans Leidekker | 2008-08-20 | [winhttp: Use default values for verb, object and version parameters in WinHttpOpenRequest. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=70fb4ef523d1d42181560f0660ec8365fae5eb9a) |
| Hans Leidekker | 2008-08-20 | [winhttp: Implement WinHttpQueryHeaders.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f14b6afb9c63dd555bae6f28da9e14a36d98acaf) |
| Hans Leidekker | 2008-08-20 | [winhttp: Implement WinHttpAddRequestHeaders.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f1d818bf3b48fa7f430e165706fc45a73b33f08) |
| Hans Leidekker | 2008-08-20 | [winhttp: Add a stub implementation for WinHttpSetTimeouts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcb0e3a9d11c074bce9c98a45fa08cbf366e6df3) |
| Hans Leidekker | 2008-08-20 | [winhttp: Deliver status notifications to the application.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6b9f60da792141decb07c1c38de3e807f52901b9) |
| Roy Shea | 2008-08-20 | [mstask/test: Conformance test for CreateTrigger.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b3b540d8b0e9cfd5bf18740d88bc2d477f0d99f) |
| Roy Shea | 2008-08-20 | [mstask/test: Conformance test for (Set|Get)ApplicationName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32354497f73703657de85f04532ea3093585ac68) |
| Roy Shea | 2008-08-20 | [include: Added defines used by TASK\_TRIGGER members.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1bc0cdded184d6e8a734ec9c91a3a229f8f9b980) |
| Roy Shea | 2008-08-20 | [include: Add task scheduler specific error codes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5331fa49d9dd7eb0233cbb6a6f7865c5cb7a4df5) |
| Hans Leidekker | 2008-08-19 | [winhttp: Implement WinHttpTimeFromSystemTime and WinHttpTimeToSystemTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=250cac32ca5ff4e7c282bd25abb4f1ae171476b8) |
| Hans Leidekker | 2008-08-19 | [winhttp: Forward WinHttpCrackUrl and WinHttpCreateUrl to wininet for the time being. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=877d6c95c6e341cf3fc5f968fb4f88509c0b6937) |
| Hans Leidekker | 2008-08-19 | [winhttp: Add stub implementations for WinHttpGetDefaultProxyConfiguration, WinHttpGetProxyForUrl and WinHttpSetDefaultProxyConfiguration. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=587162c3b6ffe0dc977fbd037521234f52e42f39) |
| Hans Leidekker | 2008-08-19 | [winhttp: Implement WinHttpSetStatusCallback. Start sending notifications.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3d9df7d4d6ab85a44468494c79251a26c692503) |
| Hans Leidekker | 2008-08-19 | [winhttp: Implement WinHttpOpenRequest.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce00aa019f344403a41eb56f9ed8799a97304b26) |
| Hans Leidekker | 2008-08-19 | [winhttp: Implement WinHttpConnect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=770ee20461ba7a262f291a7c295ec2dfbd32333d) |
| Hans Leidekker | 2008-08-19 | [winhttp: Implement WinHttpOpen and WinHttpCloseHandle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=405e8cda4116e6ecbc52b91031100f57cce205d7) |
| Hans Leidekker | 2008-08-19 | [winhttp: Add a handle management implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5c0ccf93aed9f2d61734d2f8d3e2f5bee6744e7) |
| Jacek Caban | 2008-08-19 | [mshtml: Use heap\_alloc\_zero for HTMLWindow allocation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=984bff499edcd915cbd8ae6e9f7529ef3c89b0fd) |
| Roy Shea | 2008-08-19 | [mstask: Stub implementation of Activate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=77ea6ef814a2dff8c9ccc43b7de1af1140e2081c) |
| Roy Shea | 2008-08-19 | [mstask: Activate conformance test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=75e043ee5f7b5fbf43d74ce561cd0764e51d806a) |
| Zac Brown | 2008-08-19 | [winhttp: Add test for adding/querying headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfd9681fabd386a05d3d3a1754706bc0f46c3968) |
| Zac Brown | 2008-08-19 | [winhttp: Add stub implementation for WinHttpAddRequestHeaders.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db0b7beffa21aaa1038e37c67fe60b5362ba68b5) |
| Zac Brown | 2008-08-19 | [winhttp: Add stub implementation for WinHttpQueryHeaders.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9dd04bfc32f2ae92143fdeb3b19f5ec7f53a289a) |
| Zac Brown | 2008-08-19 | [winhttp: Add test for WinHttpTimeToSystemTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=525037d758a12e301fd3ba71acdad9850b80b289) |
| Zac Brown | 2008-08-19 | [winhttp: Add stub implementation for WinHttpTimeToSystemTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=59397fab0265efbb12b44f6e1d66faf1e4342efc) |
| Zac Brown | 2008-08-19 | [winhttp: Add test for WinHttpTimeFromSystemTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5706b84513dd54e1b3ff5a1ef6914eed359595c0) |
| Zac Brown | 2008-08-19 | [winhttp: Add stub implementation for WinHttpTimeFromSystemTime.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6858aa4a0fb1c326c1eb439fc07ccda140ea44d3) |
| Maarten Lankhorst | 2008-08-19 | [winmm: Test opening the same device twice.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a7127bfc201ff7a218795c239d5b2571ea413d7) |
| Maarten Lankhorst | 2008-08-19 | [dsound: Remove int24\_struct from conversion routines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=179990ac36024b8f6054b68aa9849cc8a4cfd57e) |
| Maarten Lankhorst | 2008-08-19 | [winealsa.drv: Fix compiler warnings and remove deprecated calls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3995627de204284de96d50d3a42291f02e42c344) |
| Lei Zhang | 2008-08-18 | [shell32: Handle directories in ShellExecute.](http://source.winehq.org/git/wine.git?a=commitdiff;h=215f6c47caf16f966809b92002619adb622d30df) |
| Lei Zhang | 2008-08-18 | [comctl32: Add a test for TTM\_GETTEXT.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc6553973f02cbd763f043847498190a03e654f1) |
| Maarten Lankhorst | 2008-08-18 | [winealsa.drv: Add ability to recover from underruns to directsound driver.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2cd620802a3a7a1011a89c301270737ac1a1cfe5) |
| Dan Hipschman | 2008-08-18 | [advapi32/tests: Add tests for GetSecurityInfo with a NULL security descriptor...](http://source.winehq.org/git/wine.git?a=commitdiff;h=80c6099b2c61314bae50405a925758ea2ae75e59) |
| Dan Hipschman | 2008-08-18 | [widl: Honor typedef pointer attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=790e6dcd297717a7db160c68f3077c2a8a4c9718) |
| Dan Hipschman | 2008-08-18 | [advapi32: Implement GetSecurityInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62e5b6270ba3526bcbf4c3880ddd10be69fe2e44) |
| Roy Shea | 2008-08-05 | [mstask: Task stub with AddRef, QueryInterface, and Release.](http://source.winehq.org/git/wine.git?a=commitdiff;h=777c2f1d4649d9e5f1a3b78737cdc6a72590d26c) |
| Roy Shea | 2008-08-05 | [mstask: Implemented NewWorkItem.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f366935d55ec3dfaf695f3f726037bbe18c7c12) |
| Dan Kegel | 2008-08-05 | [shell32/tests: Test whether SHGetFileInfo should clear hIcon.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0864c55eb9713966e78df5297beb3f436261a82) |
| Roy Shea | 2008-08-04 | [mstask/test: NewWorkItem conformance test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41da56a05f0c7eb362b0d99041ac23f4d5ed5f91) |
| Jacek Caban | 2008-08-01 | [mshtml: Added IHTMLElement::get\_offsetHeight implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e273bf1f43d69b64d1b0f5e44ee21787a06c07df) |
| Zac Brown | 2008-08-01 | [winhttp/tests: Add test for sending request.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ead5566485aa3b4fcbad9ea16facce31b73ccdc) |
| Dan Kegel | 2008-07-31 | [wininet: HTTP\_QUERY\_RAW\_HEADERS\_CRLF length shouldn't include nul.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1e7f89194cec6693cea3c4fdec5702d8ccaa7eba) |
| Lei Zhang | 2008-07-30 | [cmd: Check the return value from HeapAlloc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e6bce797d3b1f13495637862e1b01fc8e5b41e3c) |
| Dan Hipschman | 2008-07-30 | [kernel32/tests: Add tests for undocumented default timer queue &quot;features&quot;.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54752c4f873e0ef940ede8767cabb9f7445fcb05) |
| Dan Hipschman | 2008-07-30 | [ntdll: Add support for a default timer queue.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a148e190af1ad0c62190e8eb1299b78abc9a9cbf) |
| Jacek Caban | 2008-07-29 | [mshtml: Forward IHTMLTextContainer::get\_scrollTop to IHTMLElement2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=985115d804ba62893fbc82307686f964ede10198) |
| Jacek Caban | 2008-07-29 | [mshtml: Added IHTMLElement2::get\_scrollTop implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4d89c62eab07ec1830f28a0e994052e0e2bcc070) |
| Jacek Caban | 2008-07-29 | [mshtml: Forward IHTMLTextContainer::get\_scroll[Hight|Width[](http://source.winehq.org/git/wine.git?a=commitdiff;h=e1a553e3283c3b1c888fa2f46496ac711aea09ad)] implementation to IHTMLElement2. LONG] |
| Jacek Caban | 2008-07-29 | [mshtml: Added IHTMLElement2::get\_scrollWidth implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=925dbb58db2e38bec53318e52d3abf6cd213f8c7) |
| Jacek Caban | 2008-07-29 | [mshtml: Added IOmNavigator::get\_platform implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=158488fdc94b140c4b6530c6592a8347431946aa) |
| Jacek Caban | 2008-07-29 | [mshtml: Added IHTMLElement2::get\_scrollHeight implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e345794235401ba42082a794033c90e7fad92df) |
| Zac Brown | 2008-07-29 | [winhttp: Add stub implementation for WinHttpWriteData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=deb49f6f8395d74ec1824055aaab07943d6bbc2b) |
| Roy Shea | 2008-07-29 | [mstask: Implemented DllRegisterServer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e5bfbfe17d71605973f16ed25d30934948ea1b6) |
| Roy Shea | 2008-07-29 | [mstask: Implemented DllUnregisterServer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=152ba903b85b5be950a8e69add824b205b4172e7) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Fix support for files with multiple odml indexes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=94ef37400ddd9f413b96549b2a37969cf9467a23) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Fix end of file handling when first request is already end of file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6becc9e14b0b2f07cea727deea47b307bfa7ea2b) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Pass InputPin as parameter to transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=89f4eeece3435eba38ef643d6c5dfb0d39f7348a) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Use correct media type in transformfilter's QueryAccept.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b452ced743333e8a3ba4a1dc560b5912192d8d4) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Make transform filter return hresult from running/pausing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db2ccf43d4e9fc5ca1a418df6c9c83a054125dd1) |
| Maarten Lankhorst | 2008-07-29 | [quartz: Trace the iface pointer in the memory allocator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa38a7e313afaa04a78c736ed8f82bb379fbebfd) |
| Maarten Lankhorst | 2008-07-29 | [uuids: Add MEDIASUBTYPE\_AYUV.](http://source.winehq.org/git/wine.git?a=commitdiff;h=668be5c7578a1b66f78245f1651e85f10644f5c8) |
| Maarten Lankhorst | 2008-07-29 | [qcap: Make the server directly register a filter instead of the workarounds.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6032ab4f175a21dfb5d49885133cc3a9bd70d0df) |
| Zac Brown | 2008-07-29 | [include/winhttp.h: Add WINHTTP\_TIME\_FORMAT\_BUFSIZE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72d201b03733e28e2b8e6891b18ae9e0af0c2ab4) |
| Dan Hipschman | 2008-07-28 | [ntdll: Fix a small timer-queue bug whereby a deleted timer may still expire.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b287a4489c6eded2f156ab3dc1c41ce319be433) |
| Dan Hipschman | 2008-07-25 | [ntdll: Implement the timer queue thread.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ef54c4cec4d89c55918559b651e83481019b7dc) |
| Dan Hipschman | 2008-07-25 | [ntdll: Implement RtlDeleteTimer for kernel32's DeleteTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c64d0cdfa5a81724307e6a71cfbb4e67fea9075) |
| Dan Hipschman | 2008-07-25 | [ntdll: Implement RtlUpdateTimer for kernel32's ChangeTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=396e47ef5c201ff01f2eef7fcb0339520db4e6fa) |
| Jacek Caban | 2008-07-24 | [mshtml: Added IOmNavigator::get\_appCodeName implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2609e45c31263253d3e3c7d36f996971a236a25a) |
| Jacek Caban | 2008-07-24 | [mshtml: Added IHTMLDocument2::[get|put[](http://source.winehq.org/git/wine.git?a=commitdiff;h=e629e049dbb22d114a863db1484f8e8dfc23d2f5)]_title tests.]_|
| Dan Kegel | 2008-07-23 | [winmm/tests: Test mciSendString with non-null return string buffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f164d504b966a8c67db68497e1c11473e583dbc) |
| Zac Brown | 2008-07-23 | [include/winhttp.h: Add remaining flags.](http://source.winehq.org/git/wine.git?a=commitdiff;h=34a17650f32ee977a340121511e3baf6df33e0fc) |
| Lei Zhang | 2008-07-23 | [gdi32: Glyph advances should be measured for unrotated characters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b4f17f630c70c320d7ac5385ec4844d9ea9cb75) |
| Lei Zhang | 2008-07-23 | [gdi32: Add a test for font orientation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=78a1e07c9344fd75eee4a95cfb949764ad8afc05) |
| Dan Hipschman | 2008-07-23 | [include: Add WT\_TRANSFER\_IMPERSONATION to winnt.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1a5011bb260f47c2a87e4f069af046253493500) |
| Dan Hipschman | 2008-07-23 | [ntdll: Implement RtlCreateTimer for kernel32's CreateTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d343f2baf76413eb690cbc44a0d56ed39915328d) |
| Roy Shea | 2008-07-23 | [mstask: Implement ClassFactory, DllGetClassObject, and DllCanUnloadNow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dab039630cc52f1633d6f878b4ee8a8866d3a490) |
| Dan Hipschman | 2008-07-22 | [ntdll: Implement [Rtl[](http://source.winehq.org/git/wine.git?a=commitdiff;h=20a1ca2bbfe1c79f2971e55ba18fa4dcab06426b)]Create/DeleteTimerQueue[Ex[.md](.md)].] |
| Dan Hipschman | 2008-07-22 | [kernel32/tests: Check that timers are not NULL in timer queue tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=09f4ca64e27103717c8455a1a3cd270d275c5062) |
| Dan Hipschman | 2008-07-22 | [kernel32/tests: Add tests for Change/DeleteTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf0f78b11a3e99004483a2b73bd915d587572eed) |
| Dan Hipschman | 2008-07-22 | [kernel32: Add a stub for ChangeTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ecd76fb77c91c9d46913c064f72b85e196ef6ccc) |
| Maarten Lankhorst | 2008-07-22 | [quartz: Fix end of stream handling in avi splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3376ba6113f81a420c56292f25bb5420ae2b6465) |
| Lei Zhang | 2008-07-22 | [ntdll: Use our own implementation of atoi and atol.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee60c49dd63fc65b9eb6813cb910ba581d80758d) |
| Lei Zhang | 2008-07-22 | [ole32: Silence FIXME from CoGetContextToken stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c7ce692d139af1a5b7e4c6db00ef4750053f58ed) |
| Lei Zhang | 2008-07-21 | [gdiplus: Add tests for passing negative strides to GdipCreateBitmapFromScan0.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a27f8b665e4bc23a448cc709de000baa42d4439) |
| Roy Shea | 2008-07-21 | [mstask: TaskScheduler stub with AddRef, QueryInterface, and Release.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f392cea55f1160d6dc35d05c393862e3edf8808) |
| Roy Shea | 2008-07-21 | [mstask: Generate C file with GUID definitions from mstask.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=21fd0a0460d218ed2c25037a80e7c38b5235dbed) |
| Dan Kegel | 2008-07-21 | [tools: Allow running tests with valgrind.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d18cd895674dc7cac1a5155f2c4b65752818743f) |
| Lei Zhang | 2008-07-21 | [gdi32: CreateDIBitmap should check for SetDIBits failure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce552d4451ffecbb3c61eeb3982541a56872bae3) |
| Lei Zhang | 2008-07-21 | [winex11: X11DRV\_DIB\_[GS[](http://source.winehq.org/git/wine.git?a=commitdiff;h=e031ef4807fdcda10d60c27dd0058232cd4abbe8)]etImageBits should return 0 on failure.] |
| Lei Zhang | 2008-07-21 | [oleaut32: Check return values in several functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fe68a9e1e8a4267217e9b2808d32f67c4411df4) |
| Maarten Lankhorst | 2008-07-21 | [quartz: Fix bugs that occur during connection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=271ee48301838dd549d368100bfcf63cb7a8df48) |
| Maarten Lankhorst | 2008-07-21 | [quartz: Fix handling of zero byte samples and endofstreams.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f9356eb16cceba6f39f4be5a5d865ccff2af56c) |
| Maarten Lankhorst | 2008-07-21 | [include: Fix typo in vmrender.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a4dcea213f9633bb8330f508beb83da6ea04c8f) |
| Zac Brown | 2008-07-18 | [winhttp/tests: Add test for opening request.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2be840e47b2f967031e1bbf8e111ecc991869df) |
| Zac Brown | 2008-07-18 | [ntdll: Remove byte reversed U+3000 (CJK space) from being checked in...](http://source.winehq.org/git/wine.git?a=commitdiff;h=38f6dbc55ac0f3e85b4e9ff06c0048b1e6807270) |
| Jacek Caban | 2008-07-17 | [msi: Added Session::Message implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=014b96ef15db221af72bb5de408dbdca4363b7f4) |
| Lei Zhang | 2008-07-17 | [user32: Clamp newly created windows to the minimum window size.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b3f4091b47e70681a9909bfccd19dee95657fabd) |
| Lei Zhang | 2008-07-17 | [user32: Add a test for SetWindowPos.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ffd66dc6abddf9e6ae2414ed0dea46faa9aa6fac) |
| Dan Hipschman | 2008-07-17 | [kernel32/tests: Add tests for timer queues.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc325c7674297ddee4085e6d5f8faa2d95f26903) |
| Roy Shea | 2008-07-16 | [mstask: Skeleton implementation of Task Scheduler Service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=80ee225f23ea8093f57f1e7b29b7fb60e6f6cdda) |
| Maarten Lankhorst | 2008-07-16 | [quartz: Fix wrong assignment of variable in parser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5299795a8dd55c81e40208eb9a57e5cb64e3732e) |
| Dan Hipschman | 2008-07-16 | [kernel32/tests: Fix p\_BindIoCompletionCallback declaration so it compiles with...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c70e6125bf7a3ee8d15b42f47d38527e7e960370) |
| Dan Hipschman | 2008-07-16 | [libs/wine: Avoid over-allocating memory in default\_dbgstr\_wn.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1b392bfa069eb43f0d6a65a4d623c95b6f624d85) |
| Maarten Lankhorst | 2008-07-16 | [quartz: Explicitly handle wave headers in avi splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ad7198961d25e30f55c9de333e01f8a2c9ceb48) |
| Maarten Lankhorst | 2008-07-16 | [winemp3: Be more tolerant to what a valid mp3 header is.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f53f5ebd8121ee1cdc88ba7db969720857051ac5) |
| Jacek Caban | 2008-07-14 | [mshtml: Added IHTMLElement2::getElementsByTagName tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1c1f8e206f62ff8f54f3a2a5f3f67d4c8d813072) |
| Jacek Caban | 2008-07-14 | [mshtml: Added IHTMLElement2::getElementsByTagName implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=952a54cbd933dbee18cbcc88521db11fb4ee7747) |
| Jacek Caban | 2008-07-14 | [mshtml: Allow timers to be cleaned during processing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1de0055cc0d47088cb9011954cf3f05b014156fa) |
| Maarten Lankhorst | 2008-07-14 | [quartz: Fix reference leak in avi splitter on end of stream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=28d6203ca9bd0ba17ce38e309f340b518f954c08) |
| Maarten Lankhorst | 2008-07-14 | [quartz: Only allocate 1 buffer in transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e9704b02dfa0d0bdb1af4941cebddde84a2af0e) |
| Maarten Lankhorst | 2008-07-14 | [quartz: Fix memory and sample leaks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf1d2f5e42fe418b0a66984bb9b0bf9134c23f20) |
| Maarten Lankhorst | 2008-07-14 | [quartz: Fix incorrect use of mtCurrent in transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=36418d8ad162df4ff237853adf5c048e830ef016) |
| Roy Shea | 2008-07-11 | [include: Add header for mstask.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c74ff3bbbcfab3bbf809095140514c2fbf3e8ef) |
| Maarten Lankhorst | 2008-07-11 | [includes: Add video mixing renderer header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=61ba32c0366c4dac79495efe3291bd538bcd4634) |
| Maarten Lankhorst | 2008-07-11 | [devenum: Call VariantInit instead of VariantClear.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ef8569c52cb58980187e3105c43ccc478c60c92) |
| Maarten Lankhorst | 2008-07-11 | [quartz: Make the file source rotate around the 'first' sample, to prevent...](http://source.winehq.org/git/wine.git?a=commitdiff;h=2865c727de7e8732fb6646d473b7818271cef0fa) |
| Maarten Lankhorst | 2008-07-11 | [quartz: End the flush downstream first before restarting playback in pullpin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=484fdcf7e446aaab859eba1b9ae79d689241592a) |
| Zac Brown | 2008-07-11 | [include/winhttp.h: Add WinHttp status codes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d778f74569ce4cc123b6ec527ef3cdcc71551e00) |
| Jacek Caban | 2008-07-10 | [shlwapi: Fixed handling mk protocol URLs in UrlCombineW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c086429465cbe9387349ef6835dfa4ac1b33e654) |
| Maarten Lankhorst | 2008-07-10 | [ntdll: Use module for path to activation context.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e98933a2795363471673fef8779112826bf13f14) |
| Zac Brown | 2008-07-10 | [wininet/tests: Change some traces to skips in tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=173cd38e68cc0857317e9f0b63d10422fe32e3f7) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Call run before pausing in transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e47bc7725e22b39d12e3408bda9f32be7d8435f2) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Make filtergraph quieter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=86393897a8da29935c145f3cd81d3f4ad56379e5) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Make parser start even if some of the pins aren't connected.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe9840f213d12967d99deda02d1c703b77a3ac94) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Fix deadlocks in dsound renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=adcf93aeaf446d657685cee8976365980499fb69) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Fix end of stream handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43d0acd26a6f396a9f2e0d90a38f5156fb86b415) |
| Maarten Lankhorst | 2008-07-10 | [quartz: Always set current position again.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6748f073ed13eec690524391ff2cd1634764a0b0) |
| Maarten Lankhorst | 2008-07-09 | [quartz: Add tests for avi splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3adf811645daaa876e1d223f98fc5428d2f79f75) |
| Maarten Lankhorst | 2008-07-09 | [quartz: Add rewrite of avi splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19360d41a0239970a7730756d7764be8f08970c8) |
| Maarten Lankhorst | 2008-07-09 | [quartz: Fix deadlock with transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=992fb02c732f8963cb70fd8167a7727911553d3d) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpCloseHandle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9575564af8eae8f455c02bf710a0fd706a8b298b) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpReadData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=058c23f77d34e0e2318d50f7c7635dc535ddcaaa) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpSetOption.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cb5908fcb7a4139896c49119b0bde944dce2ae04) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpReceiveResponse.](http://source.winehq.org/git/wine.git?a=commitdiff;h=000fe7058dc08aee65bfc9af95fb9a2131acd738) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpQueryDataAvailable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d8698918f295ad0fce40445cde5191964e5afc5) |
| Zac Brown | 2008-07-08 | [winhttp: Add stub implementation for WinHttpQueryOption.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a39e23db65db784856ac6fc6f8f92b11f1ddd18) |
| Roy Shea | 2008-07-08 | [wintrust/test: Verify array length before calling memcmp in test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=363516d7c394dac611468942a38567fc97de6a28) |
| Maarten Lankhorst | 2008-07-07 | [quartz: Only call begin process functions in transform filter when stopped.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e58855e0e913adc55df56d31020f027d55afe522) |
| Maarten Lankhorst | 2008-07-07 | [quartz: Fix tiny bug in IGraphBuilder\_Render.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e4288ee70957c3823ac7fb5879df1b130362524) |
| Maarten Lankhorst | 2008-07-07 | [quartz: Fix parser/pullpin to only care about the state transition...](http://source.winehq.org/git/wine.git?a=commitdiff;h=53782ca47acfa8e5d7ae72b59602840e3b35cd81) |
| Maarten Lankhorst | 2008-07-07 | [quartz: Make sure transform filter commits allocator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11e2b1ab2b0a867c8124a226475a12b199a1c0d5) |
| Jacek Caban | 2008-07-04 | [mshtml: Don't mix nsresult with HRESULT.](http://source.winehq.org/git/wine.git?a=commitdiff;h=047e5aaad562e65c8a976c3c86bc753d9e0ff359) |
| Maarten Lankhorst | 2008-07-04 | [quartz: Implement state transitions in video renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9985f2efc9d1e92932dd3d7f351ded3ae1db0b80) |
| Maarten Lankhorst | 2008-07-04 | [quartz: Implement state transitions in directsound renderer, and block on pause.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6b67f698a193d3c076c42dc0e3a186631e547f4) |
| Zac Brown | 2008-07-04 | [winhttp: Add stub implementation for WinHttpSendRequest.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f094b4332d4941502e4dc836f1b6df2931da3ec4) |
| Zac Brown | 2008-07-04 | [winhttp: Add stub implementation for WinHttpOpenRequest and fix function...](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae1e79d43ee2ff2d6017e98757828c87706ceff2) |
| Zac Brown | 2008-07-04 | [winhttp: Add stub implementation for WinHttpConnect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca627f5b7df7cf69ed9f3623146e22c638c65eeb) |
| Zac Brown | 2008-07-04 | [winhttp.h: Add WinHTTP error codes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5db545965f8153f65b7216ebddec67fd3ee74439) |
| Maarten Lankhorst | 2008-07-04 | [quartz: Set filesource initial state to stopped.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee317b19b2a3cfb3d3558ea079738845ca1d018e) |
| Maarten Lankhorst | 2008-07-04 | [quartz: Make CLSID\_AudioRender an alias for CLSID\_DSoundRender.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b65914cf9a84922d8f62452ae6bfa5b70f97b46) |
| Zac Brown | 2008-07-03 | [include: Add more #define's for winhttp options.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d619ed4dccf658853f6731ef37c1b16914a95bc7) |
| Maarten Lankhorst | 2008-07-03 | [quartz: Fix return values in directsound renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e5767b1c023574c00a828fb02795a138064bf4e9) |
| Maarten Lankhorst | 2008-07-03 | [wined3d: Fix a deadlock that may occur during initialization.](http://source.winehq.org/git/wine.git?a=commitdiff;h=422d71f630c8f90ca280494eaef8fda7674d1c77) |
| Maarten Lankhorst | 2008-07-03 | [quartz: Fix return value for video renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=28c7b230ed84ee73bbfefe32c64ee7d8dbf270f1) |
| Dan Hipschman | 2008-07-02 | [widl: Factor a small part of the grammar.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d87bc0520f1bc6f6201b8b44bd25cf6dff69184c) |
| Dan Hipschman | 2008-07-02 | [widl: Implement type redefinition checks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6725c5d756dc6cd1dc19e7de0e0c45005a2024a2) |
| Dan Hipschman | 2008-07-02 | [include: Fix type redefinitions in IDL files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6db7ce7a6dcf8023bf4c0ffc78c0eb3271e68cb0) |
| Jacek Caban | 2008-07-01 | [mshtml: Silence common invalid FIXME.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4171385cd96dc8fee6774afdcf6861d153f54cd7) |
| Jacek Caban | 2008-07-01 | [mshtml: Ignore fdexNameImplicit flag.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fdbdaf0b91f97e840b0f1a031b8e6ad0982c124) |
| Jacek Caban | 2008-07-01 | [mshtml: Return NULL in window object's GetNameSpaceParent.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9157c6d68ac2ccaaf06ca6440ffeab0afa10f211) |
| Jacek Caban | 2008-07-01 | [mshtml: Added IHTMLStyle::[get|put[](http://source.winehq.org/git/wine.git?a=commitdiff;h=45eba140e616504e12070b5b4c461e836e7f050a)]_width implementation.]_|
| Jacek Caban | 2008-07-01 | [mshtml: Added IHTMLImgElement::[get|put[](http://source.winehq.org/git/wine.git?a=commitdiff;h=4690d6d572ea83750b1dda945264afafbb428fa5)]_alt implementation.]_|
| Jacek Caban | 2008-07-01 | [mshtml: Silence common invalid QueryInterface FIXME.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe863e0326ec28e87454b5cc5700f2c8a9860605) |
| Jacek Caban | 2008-07-01 | [mshtml: DispatchEx's QueryInterface implementation clean up.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af3d19fa0496f07669ea53b2d2f10099645d83e4) |
| Jacek Caban | 2008-07-01 | [mshtml: Added support for DOCHOSTUIFLAG\_SCROLL\_NO DOCHOSTINFO flag.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19be7d620d31de34fd86d5faa3895bebf6818659) |
| Jacek Caban | 2008-07-01 | [mshtml: Added IHTMLWindow2::get\_self implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f58b963f4bb6fc986c7161a3eca44c84ae8e57ad) |
| Jacek Caban | 2008-07-01 | [mshtml: Added IHTMLWindow::get\_window implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebb4a9b1974ec0f77a13fe1d5ca337d98c0dc187) |
| Zac Brown | 2008-07-01 | [ntdll: Implement checking for control characters in RtlIsTextUnicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f3ae2011c39d092b0c8e2e6a9aabddbd2596748) |
| Jacek Caban | 2008-06-30 | [mshtml: Added IHTMLWindow2::clearInterval implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=876153976be7ff4d128c0e5ecc70715f21ac2e6d) |
| Jacek Caban | 2008-06-30 | [mshtml: Added IHTMLWindow2::clearTimeout implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d3aa6799c16d568b7b660bd1b95fc358bec56b5) |
| Jacek Caban | 2008-06-30 | [mshtml: Added IHTMLWindow3::setInterval implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74f29f10878ef423c60121c5a383074880d844f7) |
| Jacek Caban | 2008-06-30 | [mshtml: Forward IHTMLWindow2::setInterval to IHTMLWindow3.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0d56f1058fbcf671d6f5fde23235f4c4cbe08b99) |
| Jacek Caban | 2008-06-30 | [mshtml: Added VT\_BSTR support to IHTMLWindow3::setTimeout.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44223acceb78c1c6cbe056d67d8182e1dbf9254e) |
| Jacek Caban | 2008-06-30 | [oleaut32: Added test showing need to QueryInterface on dual  interface in ITypeInfo::Invoke. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=6971db7ee32451e2add828ad8f35d0d148013ea6) |
| Zac Brown | 2008-06-30 | [winhttp: Build an import library.](http://source.winehq.org/git/wine.git?a=commitdiff;h=927335ef158e622b8af36b3d06d93c88eda9555d) |
| Zac Brown | 2008-06-27 | [shell32: Add stub implementation for SHGetIconOverlayIndex[AW[](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a42aba9da5ce57478a567a9db3cf3413ae7b442)].] |
| Maarten Lankhorst | 2008-06-27 | [quartz: Fix Render and RenderFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d54c53a4b64223cb5744571b9f56064543e385c0) |
| Maarten Lankhorst | 2008-06-27 | [quartz: Make FilterGraph\_Connect and ConnectDirect behave better.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0d1eea691cd4e39a61fa5be5b5c5592ea7c0aa76) |
| Maarten Lankhorst | 2008-06-27 | [quartz: Make removing filters work slightly better.](http://source.winehq.org/git/wine.git?a=commitdiff;h=46f4c4b4d8d440500980f8ad46f4fee5886590c4) |
| Dan Hipschman | 2008-06-27 | [user32: Redefine internal pop-up tracking flags to avoid conflicts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50b98a29466fdebca3a550e40fe5b8e9c26ec8a8) |
| Jacek Caban | 2008-06-26 | [urlmon: Make file protocol invalid URL handling behave like IE7.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c42d937402214d4d7a744ba36f18898e0b3a78ab) |
| Jacek Caban | 2008-06-26 | [mshtml: Added DOCUMENT\_NODE type support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44a314945bacb36db0d7923f20138c78e3764b88) |
| Jacek Caban | 2008-06-26 | [mshtml: Added IHTMLDOMNode::get\_parentNode implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=beeaea11763e06b2c2233c210734413c9b07e386) |
| Jacek Caban | 2008-06-26 | [mshtml: Added useful TRACEs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=337f1b73937a7ebe8de88c45bf164272ac235249) |
| Jacek Caban | 2008-06-26 | [mshtml: Added IHTMLElement::get\_offsetTop implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2617512f022f9c38f77ae4697e9ee43c1e0ecd5) |
| Lei Zhang | 2008-06-26 | [mshtml: Remove unneeded variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f023be8aa7890a7301bda88e92ca7515e1b77a40) |
| Dan Hipschman | 2008-06-26 | [riched20: Implement ITextDocument\_fnGetSelection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=36aa6c4c447f2ec2fe1b086eb9c4ace3567ea4af) |
| Zac Brown | 2008-06-26 | [winealsa.drv: Initialize a variable in MIX\_close.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7bd0c43f0384e835bb4f26c7f810fb3bf5172461) |
| Lei Zhang | 2008-06-26 | [comctl32: Use the system variable pitch font for ip address controls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=011bad8ddf0322e6909a166a505225cf62459d7c) |
| Maarten Lankhorst | 2008-06-26 | [quartz: Downgrade a fixme to a warn in dsoundrender.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3bda54bb04cd898d6f9e508a525d8758c1dfcc8c) |
| Jacek Caban | 2008-06-25 | [mshtml: Forward HTMLSelectElement's IDispatch functions to  IDispatchEx implementation. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d978d557f421c04dd602365115fca9be279dcff) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLSelectElement::get\_type implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d6c28459be7c44d9aa897f9b5ac1e523523f021) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLInputElement::put\_disabled implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9338979c11c5d85a69134d3f8baad7bc39c030c9) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLElement::put\_title implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6314becd8cf34346505974168a0d3d3142535b7c) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLElement::get\_title implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f911e240d0ba98dd26b1f28b547ce818bcdb8b53) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLSelectElement::put\_onchange implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3a9a317de928700d266cde5dda61a605ebbeeb3) |
| Jacek Caban | 2008-06-25 | [mshtml: Return NULL instead of empty string in  IHTMLSelectElement::get\_value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da8560bbf70cfba80c75eef8b8575c9e1cdb9496) |
| Jacek Caban | 2008-06-25 | [mshtml: Added IHTMLSelectElement::put\_value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2759cb80d8fc046a9b11d9a4b458758b06db73e) |
| Roy Shea | 2008-06-25 | [dsound/tests: Added additional tests of IDirectSound\_CreateSoundBuffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a4d8caed3154726736e9ba7be62dd5dd6dd3cd0) |
| Roy Shea | 2008-06-25 | [dsound/tests: Removed test depending on value of undefined variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d776828857706547e05053d7c1199028029d9c1f) |
| Zac Brown | 2008-06-25 | [ntdll/tests: Add tests for (Rtl)IsTextUnicode to verify that...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e24e7e7852704a3d4594d2fe7b3ad6913697c5c6) |
| Dan Hipschman | 2008-06-25 | [gdi32: Return the correct value from GetTextFace.](http://source.winehq.org/git/wine.git?a=commitdiff;h=92c8cac214715633459227b2d47df61a18dc8d82) |
| Maarten Lankhorst | 2008-06-25 | [quartz: Make the memory allocator emit more warnings and fix race condition.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8bedda7e1f3a9c8300b40d1473a4b43f577f527e) |
| Maarten Lankhorst | 2008-06-25 | [quartz: Create thread after connection is made.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6aabf5d39e1a5bd13d95a9ad7a9b318f775c95fd) |
| Maarten Lankhorst | 2008-06-25 | [quartz: Remove dead code from DSoundRender.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33294331d2a6b35ad834a110d7dfd57e3540b276) |
| Maarten Lankhorst | 2008-06-25 | [quartz: Handle case where ReceiveConnection is called on an already connected...](http://source.winehq.org/git/wine.git?a=commitdiff;h=cdb66444edc807c50db247d020fe568d728e45c9) |
| Zac Brown | 2008-06-25 | [mshtml: Initialize variables in a couple structs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=332733a43bccc5a48ccda12b9a8c20eea7438e4e) |
| Jacek Caban | 2008-06-24 | [mshtml: Added IHTMLDOMNode::hasChildNodes implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c592c6e748bf9a20f8d924cc34b36f18c97afb34) |
| Jacek Caban | 2008-06-24 | [mshtml: Added IHTMLDOMNode::removeChild implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3d8d052f6f5e0163aa0853cedb19905db507a30) |
| Jacek Caban | 2008-06-24 | [mshtml: Fixed argument checking in IHTMLDOMChildrenCollection::item.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91dcf287c7818eec598e69803da6f864e6b8a8c4) |
| Jacek Caban | 2008-06-24 | [mshtml: Added support to accessing child nodes by index in IHTMLDOMChildrenCollection. LONG](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d7066b264c5ba741dfacd6ff281ff2f14c3ed78) |
| Jacek Caban | 2008-06-24 | [mshtml: Added IHTMLElement2::put\_tabIndex implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8284724abcac810772d223f760050cc4950341c) |
| Jacek Caban | 2008-06-24 | [mshtml: Added IHTMLElement2::get\_tabIndex implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=807f5c78849318497163cb471d5e18898d1e811d) |
| Jacek Caban | 2008-06-24 | [mshtml: Added IHTMLElement::put\_onkeyup implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9eb4ee2e06d7865d5f7a6ffc404bd0e71fe19287) |
| Jacek Caban | 2008-06-24 | [mshtml: Added keyup event support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0848cc977f0aefaa389ba261aaa108ae94da0684) |
| Dan Kegel | 2008-06-24 | [wininet: InternetCrackUrlW: For URLs that have no urlpath, native clears...](http://source.winehq.org/git/wine.git?a=commitdiff;h=bcdb10a9edb26649c290ff384443d8c7ee8014ec) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Clear pin value if not connected.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8a023f9f860e06d10907fed03bdd6b496bb7f08) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Add support for VideoInfoHeader2 to AVI Decompressor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9009e68c5b4aa7ff3dc592e8563e53591735916a) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Only enumerate renderers if bRender is set in filtermapper.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b157969d49bd81d23b542b19d55a8c1f8bd004d8) |
| Maarten Lankhorst | 2008-06-24 | [quartz: DSoundRender shouldn't delete buffer when already connected.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d283bcdb6230f2dd255cc085d12690802cbf6527) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Have thread safety in memallocator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d43a629d05967af6fc9fd056f995b2a563f4f14) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Implement VideoRenderer\_GetCurrentImage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dae09d000c96d1f26ef20585a4eb864b8e1d9bb2) |
| Maarten Lankhorst | 2008-06-24 | [quartz: Implement GraphConfig\_Reconfigure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0bdc8bc5c115dc65a93ce1e41bfe0a2ca0fcbfcd) |
| Jacek Caban | 2008-06-23 | [mshtml: Added generic HTML event listener and use it for click  event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf51da73f6cfe5bae5f042feacdb5e93b5713835) |
| Jacek Caban | 2008-06-23 | [mshtml: Use heap\_alloc\_zero in NSContainer\_Create.](http://source.winehq.org/git/wine.git?a=commitdiff;h=97298e66ec527260f5c85bad325b7e675c3a0e47) |
| Jacek Caban | 2008-06-23 | [mshtml: Added IHTMLElement::put\_className implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47d835206708bdedb63d779614056dca17ace71f) |
| Jacek Caban | 2008-06-23 | [mshtml: Added IHTMLElement::put\_onclick implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41bdff629fb6f0fa4420d1a567f26d7894cab114) |
| Jacek Caban | 2008-06-23 | [mshtml: Added IHTMLDocument3::createTextNode implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39c7951cf1b95b76f2b9a4bf2aaad068034211dc) |
| Jacek Caban | 2008-06-23 | [mshtml: Added IHTMLImgElement::put\_src implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23ad09865e28cf9ffa4bc816514d4b858cf2a626) |
| Jacek Caban | 2008-06-23 | [mshtml: Added IHTMLDOMNode::appendChild implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19803de2b453186cac556fc6c7b64bdaf1940d40) |
| Jacek Caban | 2008-06-23 | [mshtml: Return NULL instead of empty string in  IHTMLElement::get\_className.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0497c9896154350512282668e48ba4e01e0c3172) |
| Jacek Caban | 2008-06-23 | [mshtml: Added onclick attribute support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01dc47c884b9461e50762fd9fd398509f34845b0) |
| Dan Kegel | 2008-06-23 | [user32: Fix buffer length thinko in dde\_client.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=81fee5208b90fad16e1a1d3c750e8ffe23144d8a) |
| Dan Hipschman | 2008-06-23 | [kernel32/tests: Add tests for TLS functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e22af18e7a3b0b44512d780dc9ff664c63665dcd) |
| Dan Kegel | 2008-06-23 | [msxml3/tests: VT\_EMPTY is not a string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=578870bc4dced9fda006dd55192a826b099a3a09) |
| Dan Kegel | 2008-06-23 | [kernel32/tests: Initialize a few variables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98fba5e56a8ad997f1363b792173a74278f25c0b) |
| Dan Kegel | 2008-06-23 | [gdi32: GdiConvertToDevmodeW should not refer to unintialized name bytes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32393796bb534e9cf11dd988dce88722c67f7906) |
| Dan Kegel | 2008-06-23 | [winmm/tests: Initialize MIXERLINECONTROLSA before calling mixerGetLineControlsA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=97f4fbca7e6c363e39819c33afc613eec4c65ab9) |
| Dan Hipschman | 2008-06-23 | [riched20/tests: Add a test for creating ITextDocument.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9615e2977d136d24fd8acd6dac7701d320657f7f) |
| Dan Hipschman | 2008-06-23 | [riched20/tests: Add tests for OLE interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=76ee788afa72c481c5969577d44a60d7f5de4366) |
| Jacek Caban | 2008-06-21 | [shdocvw: Added WebBrowser's IDispatch methods implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0d8b8b15c84757ac05cbc2f90ad0bdea85b4aaa) |
| Maarten Lankhorst | 2008-06-21 | [include: Add definitions for VMR-9 interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da92dcec66f34aa6d0d02812be855295f08938e2) |
| Dan Hipschman | 2008-06-21 | [gdi32: Add tests for GetTextFace.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1480126b10ba3fe5c14242ee15e75eead3e4186) |
| Lei Zhang | 2008-06-21 | [gdi32: Check for regular fonts by style instead of style name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71ed7573aaa532eecae32a90136a4e0cb67a599a) |
| Lei Zhang | 2008-06-21 | [comctl32: Support LVCF\_SUBITEM in LVM\_GETCOLUMN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4700b0bd876d4948a364dbd00ddda1def9febebc) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Implement IBasicVideo2 for the filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00beed3d9ef9f1842e9ac593d31a92f754fdb66f) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Implement IMediaSeeking in the video renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2eb66373f5eb1b881cb8016ae8ec0ac58c1d5b81) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Implement MediaControl\_GetState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29b6dbab8097108d6c20348afe889f9309d4a799) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Try to render any existing renderers before creating a new one.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aaee8a1b0e19960b1d75cc3332f6197685cb6905) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Expose some methods so that a custom allocator can be created.](http://source.winehq.org/git/wine.git?a=commitdiff;h=365bbe8343f1f5461c4f2afe2d90be4007818878) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Only query for event interface when there is a filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a9040c1f2a762c7e8dc68c240cb57fd08fee0b8) |
| Maarten Lankhorst | 2008-06-21 | [quartz: Add the ability to force a pin to use a certain renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8705402a40682b4e6d73856e196c2f6a8cbf3c8) |
| Dan Kegel | 2008-06-21 | [dsound: Don't free buffer if it's owned by alsa.](http://source.winehq.org/git/wine.git?a=commitdiff;h=025457e09be09b7a410feaa462f3d28690f85fba) |
| Dan Kegel | 2008-06-21 | [advpack: Don't close a handle if it wasn't opened.](http://source.winehq.org/git/wine.git?a=commitdiff;h=64a62d2e8f53cb004db6cebfbbac96e3bba32ae9) |
| Jacek Caban | 2008-06-20 | [mshtml: Added createElement test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb4e098c2c431610f50c9c73e22b76097e4fc480) |
| Jacek Caban | 2008-06-20 | [mshtml: Added IDispatchEx support to HTMLGenericElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0568d8c5bd3de7cbec2a06505303ae9e116c262) |
| Jacek Caban | 2008-06-20 | [mshtml: Added IHTMLGenericElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d9cb62e37f3ef2008793e871b2c26c71b3e062ec) |
| Jacek Caban | 2008-06-20 | [mshtml: Added IHTMLDocument2::createElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f13c5685b5789e2cff5fe3b6501123c64ae181e7) |
| Jacek Caban | 2008-06-20 | [mshtml: Initialize node object from child node's constructors.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fdf676ac17d6c90978486aa62706e29fa86cd1a3) |
| Jacek Caban | 2008-06-20 | [mshtml.idl: Added IHTMLGenericElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb1190a8325141702ed274f743c370f187798fa8) |
| Jacek Caban | 2008-06-20 | [mshtml.idl: Added DispHTMLGenericElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c9a7998c36871bf756c01b037da51f452e24f31) |
| Jacek Caban | 2008-06-20 | [mshtml: Better timer handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=723b745579dba79e693e190ac624f0dabd344cb5) |
| Jacek Caban | 2008-06-20 | [urlmon: Make mk protocol behave like IE7.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1aac23d89e82d14674e262dcd9b15a5f8b704bcb) |
| Maarten Lankhorst | 2008-06-19 | [quartz: Forward some messages from IMediaSeekingPassThru.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc3377d08bd3a43ba34f5c177f7b1e7464237980) |
| Roy Shea | 2008-06-19 | [user32: Initialize hdd HDDEDATA to NULL (valgrind).](http://source.winehq.org/git/wine.git?a=commitdiff;h=6cfc6bd4f36ecf09b3dca3edefaa963200625f9a) |
| Jacek Caban | 2008-06-19 | [mshtml: Forward HTMLInputElement IDispatch calls to IDispatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd5c64dc2caa60d45605d1070956bb7eb3314795) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLInputElement::put\_value implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4360ee4d8b1501a3fadd1823f7974de4886c61e3) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLElement::get\_clientHeight implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b54a3a0314a4f5daca4dfe7c4078f1b579ec2f89) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLElement2::get\_clientWidth implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1acddbf5c9c66e9dc31d782298fbe880da7f70be) |
| Jacek Caban | 2008-06-19 | [mshtml: Better stub for IHTMLElement::setAttribute with NULL  nselem.](http://source.winehq.org/git/wine.git?a=commitdiff;h=591bab3726228119e1b6eb8e789edf8df8671611) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLElement2::put\_accessKey implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6305be26b34f69862162194c89a7bb4af15ae5b4) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLDOMNode::put\_nodeValue implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=568f26959839e940cb0b9e4ea04d261c17dbc701) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLDOMNode::get\_nodeValue implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=26e23bdd0718a42fd1df07c60a6d77418ed0dce2) |
| Jacek Caban | 2008-06-19 | [mshtml: Use heap\_alloc\_zero to allocate OmNavigator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cb99eef5a866c363f0054c4af6bf06de78e6505) |
| Jacek Caban | 2008-06-19 | [mshtml: Added IHTMLElement2::focus implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=590b185e3a05fe8900a215a4d11cd4cac191f96c) |
| Maarten Lankhorst | 2008-06-19 | [qcap: Capture pin should have an IAMStreamConfig.](http://source.winehq.org/git/wine.git?a=commitdiff;h=888b98975fdb7034faf146029da296bb06f4c8a0) |
| Maarten Lankhorst | 2008-06-19 | [winemp3: Try to find a valid header instead of failing immediately.](http://source.winehq.org/git/wine.git?a=commitdiff;h=586d9e140e3934e0a88979fe269e41aeddb04b35) |
| Maarten Lankhorst | 2008-06-19 | [include: Add definitions for IAMFilterMiscFlags interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=13281501937fd3919eeaa22c2209bbad87810f0b) |
| Maarten Lankhorst | 2008-06-19 | [include: Add definitions for IBasicVideo2 interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3806ef6f28e3cd406443d9afadf3a69b9eaf9b3) |
| Maarten Lankhorst | 2008-06-19 | [quartz: Set data length in avi decompressor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9473b750bf9ab0f4320683c95cb8ab1d251911cf) |
| Maarten Lankhorst | 2008-06-19 | [quartz: Improve the directsound renderer a bit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=40c0566879d58da8020296110fe049e39df39ec6) |
| Lei Zhang | 2008-06-18 | [comctl32: Don't rearrange icons / update scroll bar when destroying a listview.](http://source.winehq.org/git/wine.git?a=commitdiff;h=59e3490cad4faa9d6d426ef4b01e576f50497e39) |
| Jacek Caban | 2008-06-18 | [mshtml: Added IHTMLStyle::put\_color implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=57c49cbb0d57c5b43442fa2cb308a2ee3b1a8cc1) |
| Jacek Caban | 2008-06-18 | [mshtml: Added IHTMLStyle::put\_background implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b53307188fe8609864dc68b6977cc08e41e03092) |
| Jacek Caban | 2008-06-18 | [mshtml: Change backslashes to shashes in URLs passed to...](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea7666a053a1aa34c511ec47c12c246f82fb8f90) |
| Jacek Caban | 2008-06-18 | [mshtml: Added more IDispatchEx tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc021a86075f9cd9c3312714290edcfc9f219920) |
| Jacek Caban | 2008-06-18 | [mshtml: Added missing tids to HTMLCommentElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=210d6a0abbfca8d4937d1db9f5d436392b26beb5) |
| Jacek Caban | 2008-06-18 | [mshtml: Use heap\_alloc\_zero in HTMLElementCollection\_Create.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da4608227fa33701931b0663c95749ced03a586b) |
| Jacek Caban | 2008-06-18 | [mshtml: Added fdexNameEnsure support to IDidpatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32ac703e306452e994a33a63a21f3f00f5e95d3e) |
| Jacek Caban | 2008-06-18 | [mshtml: Added IDispatchEx support to HTMLSelectElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1741e652b31eb718674e74336e6fb9e775dc10cb) |
| Jacek Caban | 2008-06-18 | [mshtml: Added IHTMLElement::put\_id implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=148a7d50c552aaa4b20bc05f3354c1955672c103) |
| Jacek Caban | 2008-06-18 | [mshtml: Added IHTMLElement::get\_id implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ee45b2e4a2e2c818232be03ccf3a3c88743737e) |
| Zac Brown | 2008-06-11 | [dsound/tests: Improve test for IDirectSound8\_CreateSoundBuffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4ff8a0c0a346bd636709d8e286a08b6c8005144) |
| Dan Kegel | 2008-06-10 | [d3dx8/tests: Initialize matrix before testing its value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe508a9cd77ffe5a55ec86b290a117af8684988a) |
| Dan Kegel | 2008-06-10 | [shell32/tests: Avoid buffer overflow during test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63557d572c2f3c20acbb48a8284f7ec2945ffd05) |
| Dan Kegel | 2008-06-09 | [oleaut32/tests: Initialize reserved fields to unique values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=035f1dd0b0f502675189ee7ca95284d49d164f95) |
| Dan Kegel | 2008-06-09 | [kernel32/tests: Initialize buffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b0924cf832789238006835ad213b2fb7d760d81) |
| Jacek Caban | 2008-06-09 | [mshtml: Added FIXME about QUERY\_USES\_HISTORYFOLDER in about protocol.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f6a3234bf36240baa5015ab75a32286564d70fe7) |
| Dan Kegel | 2008-06-06 | [oleaut32/tests: VariantInit() isn't enough, you have to give a value, too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3fa578220e848a930bfa4aa2124fa3ad08c80bf7) |
| Dan Kegel | 2008-06-06 | [msxml/tests: Use VariantInit, not VariantClear, to initialize new variants.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d38dc0233a60d516f90a0626c3fd7b3a68281a36) |
| Dan Kegel | 2008-06-06 | [msi/tests: Initialize buffer lengths before calling MsiSourceListEnumMediaDisks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a302ec645ca5f314f9985ac452ac70f002caf3a2) |
| Dan Kegel | 2008-06-04 | [secur32/tests: Don't free if not allocated.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06abaaf218f89a0e7add7289c42390e677ff77ea) |
| Dan Kegel | 2008-06-04 | [oleaut32/tests: Use VariantInit, not VariantClear, to initialize new variants.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a8ad5cd5587dd5e98857d7d222a4e8c8e46597e0) |
| Dan Kegel | 2008-06-04 | [msi: MsiSourceListEnumMediaDisksW: free original string, not substring.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ecfa0fbcea9340f3de8a6b3c47af72fa0157f6cf) |
| Zac Brown | 2008-06-04 | [winmm: msiSendStringW: Don't free substring after original string has already...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d62c3197b3071e00c58d6967ad88d8d234ccc266) |
| Dan Kegel | 2008-06-04 | [userenv/tests: Fix buffer overrun.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d54392ca9915d1a7ca43017774f4679e0d2dfad) |
| Zac Brown | 2008-06-03 | [ntdll/tests: Actually verify right bytes received in aio test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b483b680136944bdb59be89c27960906278c52b2) |
| Maarten Lankhorst | 2008-05-29 | [d3d9: Add a test to see whether offscreen surfaces can be locked while a reset...](http://source.winehq.org/git/wine.git?a=commitdiff;h=06f65e65d0251abc6cc3e7556e41c2c22a041935) |
| Dan Kegel | 2008-05-27 | [advapi32: Don't test buffer length if buffer is null.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0161606b538c69ad6207b7adab867d0896adc04b) |
| Dan Kegel | 2008-05-27 | [fusion: Use HeapAlloc, not strdup, to avoid malloc/HeapFree mismatch.](http://source.winehq.org/git/wine.git?a=commitdiff;h=713290ebcea57bc5f2a0b7c1a7e237a225e8fdcb) |
| Dan Kegel | 2008-05-27 | [fusion: UninstallAssembly test: Fix typo, avoid undefined value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8ad05a25fb572286b92f25e43db65e0d0175606) |
| Dan Kegel | 2008-05-26 | [winmm: Use HeapAlloc in the capture test instead of using strdup.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b608e39e1f3eeae36b190d07e14ec2a22ae14591) |
| Jacek Caban | 2008-05-26 | [mshtml: Fixed copy&paste typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e787f84b012440de7bb37d88ef0ce5051c488f77) |
| Maarten Lankhorst | 2008-05-26 | [include: Add missing RpcMgmtIsServerListening declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c77f02c0311e3c1e283bc91b4d150240753d65f2) |
| Maarten Lankhorst | 2008-05-22 | [include: Update aviriff header to use the right alignment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a486ec907dda94b4e76ae605bdcda68286cc56cc) |
| Maarten Lankhorst | 2008-05-22 | [winmm: Fix valgrind warnings on exit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72be44ee7dd777903c9605d4fb455a9f5382bb77) |
| Maarten Lankhorst | 2008-05-22 | [winmm: Use HeapAlloc in the wave test instead of using strdup.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6589d9ab951d132aabfa1d455263585ded6d6a52) |
| Maarten Lankhorst | 2008-05-22 | [msacm32.drv: Check for message type before comparing handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63699cf58c617de4f555fd15d45bf1062eef2e78) |
| Maarten Lankhorst | 2008-05-22 | [quartz: Initialize some uninitialized variables in the video renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5026c25e053147a7f8ef4d34981eb5c163454e2a) |
| Maarten Lankhorst | 2008-05-22 | [quartz: Do timekeeping in the avi decoder.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4e32aad01372f5624dce37c1d4699f6095d31af) |
| Maarten Lankhorst | 2008-05-22 | [quartz: Don't free memory twice in null renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d7518685e884d0d1a01230e0796cae513aa216c) |
| Maarten Lankhorst | 2008-05-22 | [ntdll: Give earlier notify to valgrind that HeapFree is trying to free some...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a9a852faa9611bf155d151dab3d1bc943b99fa4f) |
| Lei Zhang | 2008-05-22 | [wininet: Send https scheme to proxy server when appropriate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd58463eda8e94deb75efa393ff7574d02c7e717) |
| Lei Zhang | 2008-05-22 | [mshtml: Added ProxyEnable / ProxyServer handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=09e8a3328943d83c05c977ba21ad8a66577e6fe8) |
| Dan Kegel | 2008-05-21 | [d3d9/tests: Another wee bit of slop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83da377494a6dfa710088b53c7791ebc0b4b62b6) |
| James Hawkins | 2008-05-20 | [msi: Check that the file key is valid before installing the assembly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70cd6bfbbd85e9caab0ec9e01314d605588eb109) |
| Lei Zhang | 2008-05-19 | [wine.inf: Open xml files using winebrowser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e63bd4dea70db985f2484124355cf18053eb3259) |
| Lei Zhang | 2008-05-19 | [explorer: Allow explorer with no arguments to run winefile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b11156b84a60eb55c1bff13ac192f718baaa2440) |
| Dan Kegel | 2008-05-19 | [d3d9/tests: Add missing skip().](http://source.winehq.org/git/wine.git?a=commitdiff;h=480297336b13ce86236148c80ed073e09fc52483) |
| Dan Kegel | 2008-05-14 | [ws2\_32/tests: Cannot reliably detect bad hostnames in &quot;modern&quot; internet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=95beaa21b87a6eec19dc788652ee2c87621996ea) |
| Dan Kegel | 2008-05-14 | [kernel32: comm.c: increase time slop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fbaf0375815ee68929f0e044c7941c08761eb3ec) |
| James Hawkins | 2008-05-14 | [msi: Copy the assembly file directly if it's not compressed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9460ae35b5401e3bdcb4db0cba00c3e3803aa99f) |
| Dan Kegel | 2008-05-13 | [d3d9: shademode\_test: Increase slop in color comparison.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d989b7f7199b3551976bcdeace91e9a18550361) |
| Maarten Lankhorst | 2008-05-13 | [quartz: Reset time when rejecting sample in the mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98f0b5f4797fba0af51411c639c87d4c76d39a6a) |
| Maarten Lankhorst | 2008-05-13 | [quartz: Silence a fixme.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d6e28c3bbc612ef2f7d2e70ab8fd4b273ea4be1) |
| Lei Zhang | 2008-05-13 | [quartz: Check input in MediaControl\_GetState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4d0d4fe360759dcfabd2c8857cd81f19ee19a3b) |
| Jacek Caban | 2008-05-13 | [mshtml: Fixed a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e497a9b0864fca9fae42fadb2201871359e5e18) |
| Maarten Lankhorst | 2008-05-12 | [quartz: Don't return a pin in filesource when there is none.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c83a63d4b678f9d54ef2bb2560e8b390ff4cb61e) |
| Maarten Lankhorst | 2008-05-09 | [winealsa: Remove calls to deprecated functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8bdebde3dc94baf1439697306e6f797ca5c7ad2) |
| Lei Zhang | 2008-05-08 | [wininet: Handle NULL input for FindCloseUrlCache.](http://source.winehq.org/git/wine.git?a=commitdiff;h=255eebe44d7cc157f7ff3c5c8d6ea8ba29d0e873) |
| Alexandre Julliard | 2008-05-08 | [services: Send the service name in the control requests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33914a1bf426f0d0d0670263b5b9f6fb24a87251) |
| Maarten Lankhorst | 2008-05-08 | [kernel32: Fix temporary path test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=864e24d2e586b796c2069576ca6d8fe4e7b8cef7) |
| Maarten Lankhorst | 2008-05-08 | [kernel32: Fix process tests to pass in Windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db8e63af27b75d098db6f9a61a6fb0ab7d70d83f) |
| Maarten Lankhorst | 2008-05-07 | [ntdll: Fix file test to not free memory allocated on the stack.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b574c11582eac45499e7a78fcbe654ad897dd94b) |
| Maarten Lankhorst | 2008-05-07 | [ntdll: Fix some exception tests to pass on Windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c509234bc7d3d615da60b80e5c7c528d5858c0c) |
| Maarten Lankhorst | 2008-05-07 | [rpcrt4: Fix ndr\_marshall test failures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd7b277d8ac23706b1c819d2ed1fd0ee9833fd06) |
| Maarten Lankhorst | 2008-05-07 | [wininet: Ignore INTERNET\_STATUS\_DETECTING\_PROXY messages in the http test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11a0e45304e9d9d69b1a2d9a6f6aa8a276f35f4c) |
| Maarten Lankhorst | 2008-05-07 | [winetest: Fix CreateProcess so that debugger tests run without timing out.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c051f13941b15bd0a399431e36cae16b8fe092e) |
| Maarten Lankhorst | 2008-05-06 | [winetest: Fix CreateProcess so that debugger tests run without timing out.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c79c2e88ce436a909caea3ad2bd3066d31415e7) |
| Maarten Lankhorst | 2008-05-06 | [netapi32: Fix test crash occuring when NetWkstaUserGetInfo fails.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a61ef431b8fe9593970aff497a6756a231df8657) |
| Maarten Lankhorst | 2008-05-06 | [winmm: Make mixer test less strict so it passes with SoundMAX drivers on XP.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc777c0ed3adc1f3a81a45fca083595439b2ad75) |
| Maarten Lankhorst | 2008-05-06 | [gdi32: Make mapping test slightly less strict so it passes on windows XP.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f74075b776e4118a8522a2ba6e11623cba9ca7bd) |
| Maarten Lankhorst | 2008-05-05 | [netapi32: Make the tests pass under XP that enforces a strict password policy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a2d53016b5ac4c214379b33663d8261311aeab89) |
| Maarten Lankhorst | 2008-05-05 | [winex11.drv: Fix a compiler warning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d50b5cef5e0c9296cc9855477615b69ed1d337c) |
| James Hawkins | 2008-05-05 | [fusion: Add the missing assembly table structs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f52ecfe0411ce891d378169f5543bc9c06753693) |
| James Hawkins | 2008-05-05 | [fusion: The Strings stream can be without a #.](http://source.winehq.org/git/wine.git?a=commitdiff;h=56bfe2972fccc12430baa3f8750135960f0054e3) |
| James Hawkins | 2008-05-05 | [fusion: Fix the type of an assembly struct member.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4442306a847af82a03a5b579f752968c8623b24f) |
| Jacek Caban | 2008-05-05 | [mshtml: Added DispHTMLSelectElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7584f2793d320dfef441f6dc6b0b3d455a80a4ad) |
| Jacek Caban | 2008-05-05 | [mshtml: Added IMG element tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29d8c366bb278a6b73c3669817063087d7cd080d) |
| Jacek Caban | 2008-05-05 | [mshtml: Added more script tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19ec36c92b37725f70dbdd63303f7a51b91a238d) |
| Alexandre Julliard | 2008-05-05 | [services: Fixed the result check for the control mutex wait.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d760cba09095221c9f5ebf1e05c3194ad5bda8e2) |
| Alexandre Julliard | 2008-05-05 | [services: Use the correct invalid handle value for the control pipe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ae87c7f0ec59fb82f6e4cd5558581ca7fc24a11) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IDispatchEx support to HTMLImgElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f263b637a99dbe749f7d3ef98c3ee2d9e9a7721c) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IHTMLImgElement stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6279de21f35b0aa17aa1cf9abaadf976b5c55624) |
| Dan Hipschman | 2008-05-01 | [gdi32: Add font faces to families in a specific order.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3537c4086b52201f1158a68d6b4aab59b76af87) |
| Maarten Lankhorst | 2008-05-01 | [quartz: More filesource fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4cdfdac35928cb4a6ad867078f01a9d2398092a) |
| Maarten Lankhorst | 2008-05-01 | [headers: Add some extra defines to vfw.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9cc32202edf4aa361b40b1f8a6bc14a7def8a556) |
| Maarten Lankhorst | 2008-05-01 | [quartz: Get rid of the sample holding code in the wave parser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8099a624697dbf1a72c58e95fa960f3355345aef) |
| Maarten Lankhorst | 2008-05-01 | [quartz: Silence a fixme that isn't.](http://source.winehq.org/git/wine.git?a=commitdiff;h=753ac6f0159c82c8cb1cd99f221615707f309d6c) |
| Maarten Lankhorst | 2008-05-01 | [Revert &quot;quartz: Handle failures better in acmwrapper.&quot;.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4afc2ae9511a45f995cf6a9246ec57dd2a185e03) |
| Maarten Lankhorst | 2008-05-01 | [quartz: Clean up pullpin code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3066116f76c0c44950fde3552485b37dce24d1f8) |
| Maarten Lankhorst | 2008-05-01 | [quartz: Get rid of the sample holding code in the mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f73bbad8ca65d7db2f225cc23481811203c355d) |
| Lei Zhang | 2008-05-01 | [userenv: Add tests for environment variables for CreateEnvironmentBlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed50b7746d99a50f985a9c7c20b5e17d1e2deb6e) |
| Lei Zhang | 2008-05-01 | [userenv: Add more tests for environment variables for CreateEnvironmentBlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf02fa309bcc08686d7751c51f08c33b74de33f6) |
| Lei Zhang | 2008-05-01 | [userenv: Add a test for variable inheritance for CreateEnvironmentBlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f7bae5af8f1d661155bdd8f4661fc8b09d5bcea) |
| Jacek Caban | 2008-05-01 | [mshtml: Handle COMMENT\_NODE like ELEMENT\_NODE in element collection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cfb8975444eed4994df10bb99fbd4b2ac62c49a1) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IDispatchEx support to HTMLCommentElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cecb2652486ee7e2b1110f387e1ee59f06a2f61d) |
| Jacek Caban | 2008-05-01 | [mshtml: Added get\_childNodes implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2db03120403cee27ca2ace5f010b7d74b6c16e2) |
| Jacek Caban | 2008-05-01 | [mshtml: Don't assume that nselem is valid in HTMLElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af529308f3bc1d4711778cf24e972e277d996f5e) |
| Jacek Caban | 2008-05-01 | [mshtml.idl: Added DispHTMLCommentElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac00714c401c6060b2a697f12adb541cad089ca2) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IDispatchEx support to HTMLStyle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9483760b35355024f892d85af35d1a3034079b9d) |
| Jacek Caban | 2008-05-01 | [mshtml: Moved IDispatchEx initialization to HTMLElement\_Init.](http://source.winehq.org/git/wine.git?a=commitdiff;h=791dd9558e67cee1b26c4029f5ef687ea2e32527) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IHTMLDOMChildrenCollection::item implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6da1c730476930f086286ef02de9aa71f6f79914) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IHTMLCommentElement stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=67333a2a19e78a0d1fc35f65181a3c9a1a4d5d44) |
| Jacek Caban | 2008-05-01 | [mshtml: Added comment and childNodes test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=57a373afb36d2efb5fe0c7827b0ab848aa6e06aa) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IHTMLDOMChildrenCollection::get\_length implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ff929ebeb9ab1aff3fdc8b0dd2d3a2119096c72) |
| Jacek Caban | 2008-05-01 | [mshtml: Added IDispatchEx support to HTMLDOMChildrenCollection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30d204753704cc1ff4c714e274effba98d1a21b5) |
| Lei Zhang | 2008-04-30 | [userenv: Initial implementation of CreateEnvironmentBlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bca84d5467bc0242da027d24082871d8df3053fd) |
| James Hawkins | 2008-04-30 | [msi: Add initial implementation of MsiPublishAssemblies.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bfe07d1d07c9469a398858d0f077e26c26695b5d) |
| Jacek Caban | 2008-04-30 | [mshtml.idl: Added DispHTMLStyle declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e487b1e213acf3b77c3e62fb0c670817b5be91d9) |
| Jacek Caban | 2008-04-30 | [mshtml.idl: Added DispHTMLImg implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ed14f98aab2b896074018b6793d4f1c49d5bc32) |
| Lei Zhang | 2008-04-30 | [userenv: Add initial tests for CreateEnvironmentBlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ffb04579826c5024387ff01e7ef36b96ad092d66) |
| Lei Zhang | 2008-04-29 | [winmm: Do not unload drivers when the process is terminating.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d20f982433b6c1fe735699f3172e67d2e0a6884b) |
| Maarten Lankhorst | 2008-04-29 | [quartz: Some state changes fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e761d26135ba73bc8916fa3a3579512c1c3978b) |
| Maarten Lankhorst | 2008-04-29 | [quartz: Handle failures better in acmwrapper.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ba8ece76e1b87f43270edb1324c31b818e8162e) |
| Maarten Lankhorst | 2008-04-29 | [quartz: Keep track of the time in the video renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37847b0d9b884752e86eedc96bc3294b78a9b51b) |
| Maarten Lankhorst | 2008-04-29 | [quartz: Fix bug in memallocator with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1fad872961499c48c2b33851636f8408d67321cc) |
| Jacek Caban | 2008-04-29 | [mshtml: Added IDispatchEx support to HTMLOptionElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=928914c81ebbbb21ff66e3b044036bf7a4172d08) |
| Jacek Caban | 2008-04-29 | [mshtml: Added IDispatchEx support to HTMLInputElement.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7582518e18b50bf4ebbd2cda30822d25be3d81a9) |
| Jacek Caban | 2008-04-29 | [mshtml: Added indexed access to HTMLElementCollection object support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1597967417caa123153bec5b307f31ed7fd5fa18) |
| Jacek Caban | 2008-04-29 | [mshtml: Added support for custom DISPIDs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef4200fcf78159e1b7f1d5f87f98b054d15dbf75) |
| Jacek Caban | 2008-04-29 | [mshtml: Added IHTMLCommentElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96fdb0e7425317eece64e573f9444521194bd931) |
| Jacek Caban | 2008-04-29 | [mshtml.idl: Added DispHTMLOptionElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3186aa7a6508a03d0021c41ba1e4e1685952b892) |
| Jacek Caban | 2008-04-29 | [mshtml.idl: Added IHTMLDOMChildrenCollection and DispDOMChildrenCollection...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f885b332189f3656acd60834c677e6b76735b88a) |
| Lei Zhang | 2008-04-29 | [advapi32: Replace UuidToStringW call with a sprintfW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9fca0f27d02d88c6e8f1f8ef870ae59838eeb51d) |
| Jacek Caban | 2008-04-28 | [mshtml: Added IHTMLInputElement::get\_disabled implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e913b9551746f432fc2c96ef8a708dcf9ad3323) |
| Jacek Caban | 2008-04-28 | [mshtml: Added put\_backgroundImage implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=deeaa5d20fdf5c3fc207c044b7df8b0d0c65323b) |
| Jacek Caban | 2008-04-28 | [mshtml.idl: Added DispHTMLInputElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32846424be02af2600fee5aaadb2b9652b40902d) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Fix acmwrapper time regression.](http://source.winehq.org/git/wine.git?a=commitdiff;h=10708b405c2303e782a688edad1a79215fca142d) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Add a function that can be called when stopping processing data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=512ee927cb56a6b3355550c2f929d34f080247ea) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Make dwSamplesProcessed a longlong.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ec87de35af3ccb76383697b51aefe8041bbfdc15) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Optimize the file source to do its job better.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12a0fd3d8b0acff07ec07b4d7f5ea1f79effad93) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Make the EnumPins interface dynamic.](http://source.winehq.org/git/wine.git?a=commitdiff;h=79349513435aa677e584bcad66865cafbac95db9) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Fix time discontinuities in the acm wrapper.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7e20bfdd1bc9777e56cb3fe73976e38146c1741) |
| Maarten Lankhorst | 2008-04-28 | [quartz: NotifyAllocator does not like a null argument.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e143cdb6323446506444a23caf717477270dc52) |
| Maarten Lankhorst | 2008-04-28 | [quartz: Add a vtable argument to Parser\_Create that individual filters can...](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f136a57f7a54b78741540ae34378d7624bb1f3a) |
| Lei Zhang | 2008-04-25 | [user32: Edit controls should ignore WM\_KEYDOWN on control + enter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae1b735547857fd8473b7d01c6be1ee586807e6a) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IDispatchEx support to HTMLElementCollection object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=989574510cdc8627b09b6ee94d1120ed1f334f73) |
| Jacek Caban | 2008-04-24 | [mshtml.idl: Added DispHTMLElementCollection declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74c571a441545997796b790e55ccb2851c7c2aaf) |
| Jacek Caban | 2008-04-24 | [mshtml: Added get\_nodeType implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb05803a2ac56c078393803503fc73400c51c9c1) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IDispatchEx support to text node.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af271b3b45b195243a1798b4c111a94e41838877) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IHTMLDOMTextNode stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=754adce78190c726db510873af89ba389b7d2b0c) |
| Jacek Caban | 2008-04-24 | [mshtml: Added get\_firstChild implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6bf5ffbc3b26cb521b57b656c6b6f375cbab6c0d) |
| Jacek Caban | 2008-04-24 | [mshtml.idl: Added IHTMLDOMTextNode declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1cb633a5ccdf4b3b359b7bf20e2264611e02f750) |
| Jacek Caban | 2008-04-24 | [mshtml.idl: Added DispHTMLDOMText declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f731140c91c08daa13125205b1b86c00651fa34d) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IHTMLDOMNode2 to IDispatchEx support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d024a6d1db60fb3d71cdeeb3aa110b64c75e467) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IHTMLDOMNode2 stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8dc2cf0d3a7babb16cafef2f1b7636d414609597) |
| Jacek Caban | 2008-04-24 | [mshtml: Return VT\_NULL instead of empty string in getAttribute.](http://source.winehq.org/git/wine.git?a=commitdiff;h=872810e6419876c03d1d4c2a7dc69d77ab944338) |
| Jacek Caban | 2008-04-24 | [mshtml: Added more IDispatchEx tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01f241c07df211f12e1fc00c7d9e5513f0f8e2c6) |
| Alexandre Julliard | 2008-04-24 | [wine.inf: Fix the service type of the spooler service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=981f31bedf5090393b50733c09e035ddba74f934) |
| Alexandre Julliard | 2008-04-24 | [services.exe: Don't reject config changes if the display name corresponds to...](http://source.winehq.org/git/wine.git?a=commitdiff;h=af972cb1e414de53ae073d4af61c2885957b8925) |
| Alexandre Julliard | 2008-04-24 | [services.exe: Make the changed status event an auto-reset event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea746219860cc10389f04fec933ba27abe04c70d) |
| Lei Zhang | 2008-04-24 | [winex11: control + enter should generate '\n' instead of '\r'.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a442d2675e20ba1a0d5b8ea3ebded22673fa8f1a) |
| Dan Hipschman | 2008-04-24 | [wininet: Don't forget the INTERNET\_STATUS\_REDIRECT callback in HttpEndRequest.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3051cba22db94b5f419790230372d06bc53a100) |
| Jacek Caban | 2008-04-24 | [mshtml: Return S\_OK in QueryContinue.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f33fee5afd224be3fc414e5dc34a763f23cbad1) |
| Jacek Caban | 2008-04-24 | [mshtml: Fixed typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=38e9364b65866d278150efebc945a92726a10dd8) |
| Lei Zhang | 2008-04-24 | [user32: Handle VK\_RETURN WM\_KEYDOWN events better in edit controls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f0b111243609c9501c130e341871cd6dedfb515) |
| Lei Zhang | 2008-04-24 | [user32: Add a test for sending WM\_KEYDOWN to a child edit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1e5faee29e568b6c6df2b0eb3cc6d86b73ff91f1) |
| Jacek Caban | 2008-04-24 | [mshtml: Added elements IDispatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5059b8303b084ab13bb9eb042e161f12b32d164) |
| Jacek Caban | 2008-04-24 | [mshtml: Use heap\_alloc\_zero for allocating node objects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=38b14274fb507d1b6d387b38875f85720a5ee78d) |
| Jacek Caban | 2008-04-24 | [mshtml.idl: Added DispHTMLUnknownElement declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=22eb495aaf0bf0d4d3374e0e6f5890badb351bea) |
| Jacek Caban | 2008-04-24 | [mshtml: Added IHTMLDocument3::getElementById implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e610d2ff12fbb52ecd0fd17a4ade034de9b22d2d) |
| Alexandre Julliard | 2008-04-23 | [winex11: Don't allow changing the X11 size of a maximized window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bbd32aacff1555df0153deee22ca40de992de007) |
| Alexandre Julliard | 2008-04-23 | [winex11: Make sure that the window gravity is always set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ba06fa7af24922ec6b88c1ba49a46628bec5299) |
| Dan Kegel | 2008-04-23 | [gdiplus: GdipLoadImageFromStream: initialize variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c8262510dbd1595bda8970bc59b389b0597cf81) |
| Maarten Lankhorst | 2008-04-23 | [dsound: Skip WAVE\_FORMAT\_EXTENSIBLE tests on directx &lt; 8.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf739cbcc38c2ba95a0f087cb34be61f5ca395ef) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Make the file source support multiple samples by preallocating enough...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e0fe0ef01b32b06503e22310c1a54ae9c765b54b) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Make wave parser and mpeg splitter zero copy by getting rid of the...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a39805ed8345047d217f4a0d7de3954cce7cb93) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Add some sanity checks to file splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ec124be8239b6292ba239bb24f125cd4e267fdd5) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Copy discontinuity status in acmwrapper.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4abbf915d398d5a2402c7acf85d7456a488d03ac) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Fix inverted logic in memallocator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f736c4a5a6e1c652073cc5cc49b3e7bf0f42ba3) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Fix error message names in tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1e9dbcc5125bd865ad982cc94f7e36c8580faba7) |
| Maarten Lankhorst | 2008-04-23 | [quartz: Optimize the processing thread to fetch one sample while processing...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0224676905f0b96f2ade672f90cea696a5434bc) |
| Dan Kegel | 2008-04-23 | [winecfg: Restrict dpi slider to sane values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=faaccca59be08be547ec4e1948b6306eff3808a2) |
| Dan Hipschman | 2008-04-23 | [wininet: Remove custom content-length/type headers from redirects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1ebffb4527e083d3a39762851fbc3d76b5ecfa4) |
| Maarten Lankhorst | 2008-04-22 | [explorer/mountmgr.sys: Move device hotplug code over to mount manager.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c02e01dcb1ee281fac7d50bdbc5e4fb93af4971) |
| Lei Zhang | 2008-04-22 | [gdiplus: Do not access freed memory in a test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=321dfcc7a987d0be5738bdc8642d0531fb6db7d3) |
| Lei Zhang | 2008-04-22 | [gdiplus: Initialize variables in the graphics test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c9209ac0b45a7ca01ca42b04aeadb0a2219f9bb) |
| Jacek Caban | 2008-04-21 | [mshtml: Forward IHTMLDocument2's IDispatch methods to IDispatchEx...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0a32cd868db912ad861bc2269c38e595f0e7c8c3) |
| Jacek Caban | 2008-04-21 | [mshtml: Added HTMLDocument's IDispatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98ab1a92c03c9aa28963e5cb221a7fbd137bd318) |
| Jacek Caban | 2008-04-21 | [mshtml: Make IHTMLDocument2 iterface offset independent.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d0034a5ba3ab64cba7440c28d642f4e8d1e0978) |
| Jacek Caban | 2008-04-21 | [mshtml: Added setTimeout implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=788432af49d0ce9a63ab15397c5277c68ec574b2) |
| Jacek Caban | 2008-04-21 | [mshtml: Forward IHTMLWindow2::setTimeout to IHTMLWindow3::setTimeout.](http://source.winehq.org/git/wine.git?a=commitdiff;h=86409551889d99775aa04c64c48188c8cc32ad68) |
| Jacek Caban | 2008-04-21 | [mshtml: Added IHTMLWindow2::get\_document implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aeb1095b47482fdbdb46814d51a54601712837ef) |
| Jacek Caban | 2008-04-21 | [mshtml: Added navigator's IDispatchEx test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c63087a5c99c144567095ef65326350fcbd9b92) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Add some more tests and fix wine to pass them.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9c2d8e2f418fe901de82e3181491e4dd52af7ef) |
| Maarten Lankhorst | 2008-04-21 | [quartz: No longer drop packets on discontinuities.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fb2c975a8f5b54f9e7a667ee3638f340d80f2af1) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Drop preroll frames in directsound renderer too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7fbc7ef8cb92c1c7811ea70dd4c68ff21002929) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Flux AsyncReader in PullPin\_BeginFlush.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d16639d1fad14ff2b7afa43acc57d78122478432) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Add more seek entries and fix a time continuity bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1a4acde0153626095685ff1c97287cf25004087) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Only drop Preroll samples after obtaining its time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d9bf6f158cd8e9a734fddb311f3aee30ba4d486) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Change longlong printfs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=810a933f68fe458b19f7734794206151e4c3b38e) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Make the video renderer drop preroll samples.](http://source.winehq.org/git/wine.git?a=commitdiff;h=458b09a84dc168ca4a1cde927226b93ba4afff2a) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Fix sample leak in file source on failure path.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33b2f69c9fef56107665bb4ae0e915b2dcd8df13) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Make acmwrapper respect preroll samples.](http://source.winehq.org/git/wine.git?a=commitdiff;h=172347341ae4b9e23704b7cb3f6888b9f84452cc) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Fix theoretical memory leak.](http://source.winehq.org/git/wine.git?a=commitdiff;h=119d7caf79674988df6b57f6e0ee766031270ab8) |
| Maarten Lankhorst | 2008-04-21 | [quartz: Set media time in the file source.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0458c08b95d368cba6daf1f216c0e930c6387dd6) |
| Maarten Lankhorst | 2008-04-21 | [dsound: Skip the sound checks on the primary module and change its driver...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c4d9448a9d25b693693912bcb3ab0cf4274d7d3) |
| Jacek Caban | 2008-04-21 | [mshtml: Forward window IDispatch methods.](http://source.winehq.org/git/wine.git?a=commitdiff;h=951084abcf16766f8c5636738ffd614089acf793) |
| Jacek Caban | 2008-04-21 | [mshtml: Added window IDispatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5843056c5c77c522b803e8a6dcea01e725ec303) |
| Jacek Caban | 2008-04-21 | [mshtml: Forward IOmNavigator's IDispatch method to IDispatchEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=835b3eb0e81673d627a999bf57192e72d0d2032e) |
| Jacek Caban | 2008-04-21 | [mshtml: Added IDispatchEx::GetIDsOfNames implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0e0bf6b15c207ae7c1fc93497ec036e33e7a55b) |
| Jacek Caban | 2008-04-21 | [mshtml: Added IDispatchEx::Invoke implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c6ea438a00e6ad86926a5062f808517884758da) |
| Jacek Caban | 2008-04-21 | [mshtml: Added IDispatchEx::InvokeEx implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=de74e1aeb95285aea351ae8005f80c1b5350b9f2) |
| Jacek Caban | 2008-04-21 | [mshtml: Added IDispEx::GetDispID implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b81818e7ee209e49241f6d696cac6952a1ed89c3) |
| Jacek Caban | 2008-04-21 | [mshtml: Added load event support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12f312daccf5201e4b26d2d76ab4a87411821c15) |
| Jacek Caban | 2008-04-21 | [mshtml: Parse and store onload attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c21a5d3b0a4bba4029d0debc0d3b894626f5bd3) |
| Lei Zhang | 2008-04-18 | [msxml3: Check for xsltInit before calling it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d7f7bfc5e4c3c0fd1039c14df0aae44a490b3b9) |
| Jacek Caban | 2008-04-18 | [mshtml: Store IActiveScriptParseProcedure in ScriptHost.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfc84bd9642513558da3d489a1e0e029d3a23187) |
| Jacek Caban | 2008-04-18 | [mshtml: Added IHTMLWindow3 stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a009157331320cc52482089fa5eedcd8d9d15bcd) |
| Jacek Caban | 2008-04-18 | [mshtml: Added possibility to get node object from nsIDOMNode only if available.](http://source.winehq.org/git/wine.git?a=commitdiff;h=625ed3d0aa631de0b70fef0a96ba4586b7f86df6) |
| Alexandre Julliard | 2008-04-17 | [user32: Added support for WS\_EX\_RIGHT in the static control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cc82b07b344d8c0cf11f1f6efa4a4c8e52f3df3) |
| Alexandre Julliard | 2008-04-17 | [user32: Added support for WS\_EX\_RIGHT in the edit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4136deecb50643af02c520fa3f80f2473de61d1) |
| Alexandre Julliard | 2008-04-17 | [user32: Added support for WS\_EX\_RIGHT in the button control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bbd9e229e3c2676e9db7ce64d6a87bb75f506e84) |
| Maarten Lankhorst | 2008-04-17 | [server: Make enum\_desktop enumerate all the desktops on the window station with...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3fd1fc760046165e63146a2803b510079ee00035) |
| Maarten Lankhorst | 2008-04-17 | [server: Make enum\_winstations enumerate all the window stations with...](http://source.winehq.org/git/wine.git?a=commitdiff;h=81069001ea65cd517b62e2a80cd28e35be044794) |
| James Hawkins | 2008-04-17 | [fusion: Explicitly check for -1 for a missing table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e52e5e67159753cdc0c5abfa409f71c0710dab47) |
| Jacek Caban | 2008-04-17 | [mshtml: Move get\_typeinfo to dispex.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be59368dd1176becfd582d0d959e16b23430b97d) |
| Jacek Caban | 2008-04-17 | [mshtml: Added generic IDispatchEx implementation and use it in OnNavigator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed6a8acca71a37060234168aa5c755787d5dce2f) |
| Jacek Caban | 2008-04-17 | [mshtml: Added IActiveScriptDebug32 stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0d8dc2811b495914b1c1b6eb45b62ae26b2e5ac) |
| Jacek Caban | 2008-04-17 | [mshtml: Make sure to null terminate buffer in parse\_extern\_script.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2c80e6b186079200875a936f853fffeb6967206) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Obtain the duration using the index in avisplitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebaadba498a9e8d546768f0714faa3e93f3a2e57) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Store the stream index in the avi stream for files that have them.](http://source.winehq.org/git/wine.git?a=commitdiff;h=162581711375fec58cc595ab75646235d31ee099) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Check for discontinuities in the directsound renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0e8b97ffe470718a27dca98c674a3b61c16c213) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Make sure at least 1 sample is processed before returning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=97b9e9c3add01235817b172b19626718fc2a02e7) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Reject samples in transform filter only when stopped.](http://source.winehq.org/git/wine.git?a=commitdiff;h=405e21d5589c5563f9e0ab00b3ed1c9a4a498faf) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Reject samples in video renderer when stopped.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3dc8384aa9e7525877c68d742ecddb8169a20779) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Fix IMediaSample2 SetPreroll and SetSyncPoint.](http://source.winehq.org/git/wine.git?a=commitdiff;h=382a61391f30d0fd86e97a0a5d3b6c14d7a942cc) |
| Maarten Lankhorst | 2008-04-17 | [quartz: Fix discontinuities in wave parser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cbb0ff37fa63eefcf1d86ccdf894c9accc4b93b8) |
| Maarten Lankhorst | 2008-04-16 | [quartz: Add a Disconnect function to the parser and use it to clean up...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6165d87fc5d1a2147deba22e802ed41885e48635) |
| Maarten Lankhorst | 2008-04-16 | [quartz: Parse old style avi index.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa623d2eff75e03d6269bbb3c75bd296210c6181) |
| Maarten Lankhorst | 2008-04-16 | [quartz: Make the avi splitter skip index headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f66ad4dbe0433b6679d61f6a147b2cb5e3712fae) |
| Maarten Lankhorst | 2008-04-16 | [quartz: Dump opendml indexes and header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=64be38a5b20b5fe64d52e4c2464434e6b5a313d0) |
| Dan Hipschman | 2008-04-16 | [qmgr/tests: Fix minor potential memory leaks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cacd1c448e633852c77bfa87572aa12895d7e86a) |
| James Hawkins | 2008-04-15 | [fusion: Implement IAssemblyCache::InstallAssembly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=282246eca4aa778f447e8951dea416fb5e817657) |
| Lei Zhang | 2008-04-15 | [user32: Handle ctrl + end in edit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=483116a89e96430b9ce41b629e5c75b52d45e7cc) |
| Lei Zhang | 2008-04-15 | [user32: Handle ctrl + home in edit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfdd9290a7d90e11fec3a1045ad48fae6d79921e) |
| Lei Zhang | 2008-04-15 | [user32: Do checks in the right order in EDIT\_BuildLineDefs\_ML.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4aef5cb86dcb1e2692a233883f3fe102a5477334) |
| Jacek Caban | 2008-04-15 | [mshtml.idl: Added IHTMLWindow3 declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b56a072eb964f51afc8f7e34a4d18207c1f5a868) |
| Jacek Caban | 2008-04-15 | [mshtmdid.h: Fixed IHTMLWindow2 dispids.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a0a0453100e8912b74fb05059b12d292bccc9d7) |
| Maarten Lankhorst | 2008-04-15 | [include: Update aviriff header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b326924510faf14acb1fbfd024eedb5ac959803) |
| Maarten Lankhorst | 2008-04-15 | [quartz: Update start\_time if the current position is changed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1281b74956d28c2814cb5c592121410ddd1b750c) |
| Maarten Lankhorst | 2008-04-15 | [quartz: Add VIDEOINFOHEADER2 support to VideoRenderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3e9cee050f801ab3cd69378d168f5efd51862f0b) |
| Maarten Lankhorst | 2008-04-14 | [quartz: Bring waveparser to the same level as the mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebe438c82a017e20500bc7c725cb12f83f70123f) |
| Maarten Lankhorst | 2008-04-14 | [quartz: Set sane defaults for pin stream rate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8e31b5bdd2d921bf3010aec974b16e327c26479) |
| Maarten Lankhorst | 2008-04-14 | [quartz: Silence seeking fixmes on transform filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba10e6104a8f485ed40345212a325b94369525d1) |
| Maarten Lankhorst | 2008-04-14 | [quartz: Silence requests for IVideoWindow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5fb4224f81c8b18ede56dd723c68fb74b76b83a4) |
| Maarten Lankhorst | 2008-04-14 | [quartz: Don't clean up in avi decoder if driver isn't opened.](http://source.winehq.org/git/wine.git?a=commitdiff;h=48f80f629634d1bb62d1f49f4b260647c432eace) |
| Maarten Lankhorst | 2008-04-14 | [include: Add dvdmedia stub header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=271f2eda14a1345044df11deeedb735435ad1015) |
| Alexandre Julliard | 2008-04-14 | [winex11: Make WS\_EX\_APPWINDOW windows have normal type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9bf9c0b7ec6d4475962e6c739ca2f83a7a11fda7) |
| Rob Shearman | 2008-04-11 | [advapi32: Add exception handling around all service RPC calls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe7e786ace4683769e0deb0061dc69504cf0a341) |
| Rob Shearman | 2008-04-11 | [ole32: Use I\_RpcExceptionFilter instead of custom exception filter for RPC...](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa83f5a5aa5ffab8bbc25b8fb76e1dcdb5ae8a96) |
| Rob Shearman | 2008-04-11 | [services: Automatically start boot-start, system-start and auto-start services...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a35bd4971b363905491d00a4cbb152a84d27b49) |
| Rob Shearman | 2008-04-11 | [services: Split RPC\_MainLoop into initialisation and the actual loop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=559fafebbf648925bbaab61ab61894b11c90c104) |
| Rob Shearman | 2008-04-11 | [rpcrt4: Implement I\_RpcExceptionFilter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a2914b11f92f1ccb3187eb782f622cbba1e6726) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetMetafileDownLevelRasterizationLimit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54a06642f40129949475a689115383908e9b7dfa) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetLineTransform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82d01449129e3c5616eb9bc36ca2ccf80851b0ad) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetLinePresetBlend.](http://source.winehq.org/git/wine.git?a=commitdiff;h=942f3496b392113d0d3913983af6690f2400f3b9) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetLineLinearBlend.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0399cdaff0b8847b7fad13d49a7bdf42f7ac915b) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetLineColors.](http://source.winehq.org/git/wine.git?a=commitdiff;h=89b0a979c8855b09d1190df09836411d3c885b2e) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetInfinite.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0fe2f5b67716c18b074c60b341f9a7c602b41408) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetImageAttributesToIdentity.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a44f191797b6425aa11dee13027fc3a71b57aee) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetImageAttributesThreshold.](http://source.winehq.org/git/wine.git?a=commitdiff;h=03c7d5583049d59e8bae61406fe8c61d49fda928) |
| Lei Zhang | 2008-04-11 | [gdiplus: Add a stub for GdipSetImageAttributesRemapTable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=65445b9e7ebf77b4b24bda687249a67091152512) |
| Alexandre Julliard | 2008-04-10 | [winex11: Make sure to flush painting operations before moving a window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70ef99e5e115078d7d3ece8b04aabb94f701e167) |
| Maarten Lankhorst | 2008-04-10 | [quartz: Add stubs for the IMediaSeeking interface in SeekingPassThru.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd324db0597b450cff8b4bc87d20d852319d2196) |
| Maarten Lankhorst | 2008-04-10 | [quartz: Add a stub for SeekingPassThru.](http://source.winehq.org/git/wine.git?a=commitdiff;h=65e6bbd1861d403c364800c8aea29456c55680d5) |
| Jacek Caban | 2008-04-10 | [mshtml: Correctly handle NULL req in get\_nscontainer\_from\_load\_group.](http://source.winehq.org/git/wine.git?a=commitdiff;h=732682b08cf3b64267045cf0ab051fb84af43aea) |
| Jacek Caban | 2008-04-10 | [mshtml.idl: Added DispHTMLWindow2 dispinterface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f9b7741ca97798baf3d416553bfbb2c3926f450) |
| Jacek Caban | 2008-04-10 | [include: Added ICanHandleException interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea215f790dd151fdf5b13000c37c53ff183a588f) |
| Jacek Caban | 2008-04-10 | [jscript: Added IObjectSafety tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b9117b6166de3c8f27483ace5225f5c63975f85e) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetImageAttributesOutputChannelColorProfile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ba99f4eb556b4d0b3518d91404460e8b7e05e16) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetImageAttributesOutputChannel.](http://source.winehq.org/git/wine.git?a=commitdiff;h=139da784bf1bae0fa19184a3a46be1449efbee1f) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetImageAttributesNoOp.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68f5cdb28e21d20dad925737485a163833960761) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetImageAttributesGamma.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7b403d6b4680ba2d958eef5a0f2913e14ee64b43) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetImageAttributesCachedBackground.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b2db98cb6839b0baddf092ce0dd15409ec9fead) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetEmpty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d7e2254f6a9bc3a844ada910995fa58728c5bf4) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetEffectParameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=20a8cf641712289dfb96cc9cccfa5b06f1b8d970) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetCustomLineCapWidthScale.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1394d4d482c8f286b273f76d7617f1a4343edda) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetCustomLineCapStrokeJoin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1131685a94ea1e23784af7b9e5854c56df369470) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetCustomLineCapBaseInset.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af1e221f170c4c5ee6c92083c5e91d92b5f7de51) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipGetCustomLineCapBaseInset.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6112d16bad2cab5f3018af189f556f72bd718f91) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetCustomLineCapBaseCap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39e9bdbd2a1d4a5c99f0c6c246a8c60e198d0391) |
| Lei Zhang | 2008-04-10 | [gdiplus: Add a stub for GdipSetClipRegion.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cec6c2eb4df6c823998171b243e434e79e26e5c3) |
| Lei Zhang | 2008-04-10 | [user32: Handle VK\_TAB in EDIT\_WM\_KeyDown.](http://source.winehq.org/git/wine.git?a=commitdiff;h=95f323ed4666b5194816c707abc425fcf5745f6f) |
| Dan Hipschman | 2008-04-10 | [qedit: Add a stub for IMediaDet\_get\_StreamLength.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfbb2fc9e0ded9b06147f653de7e878cef3657dd) |
| Dan Hipschman | 2008-04-10 | [qedit: Implement IMediaDet\_get\_FrameRate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=953600255210c563e938b3b83277aab058613a7f) |
| Dan Hipschman | 2008-04-10 | [qedit: Implement IMediaDet\_get\_StreamMediaType.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b0d68e4093622cdf7a943cc5e3825e81176be31) |
| Maarten Lankhorst | 2008-04-10 | [include: Add ISeekingPassThru interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7fa1c9d024231847c3385a82d478a7b9f59b32cc) |
| Maarten Lankhorst | 2008-04-10 | [quartz: Implement stop position in the mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2734e6332ccceb35182c89fc8cc9d222a0b05dd0) |
| Maarten Lankhorst | 2008-04-10 | [quartz: Implement stop position in the filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43f9fff0a0237efa88de16e8a1ba7da9a58b09d3) |
| Lei Zhang | 2008-04-09 | [user32: Fix a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cc671eec57dde6659ae058af0b98b4ec1bb71eb) |
| Lei Zhang | 2008-04-09 | [user32: Add edit control check to see if its in a dialog on WM\_CHAR/VK\_TAB.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7ffa867256f7fdf886c23a93048399bd16794ed) |
| Lei Zhang | 2008-04-09 | [user32: Add edit control check to see if its in a dialog on WM\_CHAR/VK\_RETURN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f704d5c69991d59c70859c172e903318e68536c7) |
| Lei Zhang | 2008-04-09 | [gdiplus: Add a stub for GdipSetClipRectI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d9a4299bfc0d5fbc1f1cb6126f1546b49ad9118a) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Make the directsound renderer handle the Play->Pause->Play position...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2dccab7e3a836eabcc27c3c25ef935e05fd5eb8) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Generate a seek table for the mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=24cac935f05ef37405dc11b9d034efd4f7bde8f5) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Remove while { } while construct.](http://source.winehq.org/git/wine.git?a=commitdiff;h=55f3ba9dc0df257e3488968b15545418b08148b4) |
| Dan Hipschman | 2008-04-09 | [qedit: Implement IMediaDet\_(put|get)\_CurrentStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33f270afc07541293c0f7a142473a66201547ba5) |
| Dan Hipschman | 2008-04-09 | [qedit: Implement IMediaDet\_get\_OutputStreams.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3061d48e1c78c331b93be7a880876ebff2730dd) |
| Dan Hipschman | 2008-04-09 | [qedit: Implement IMediaDet\_get\_Filename.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d2d5a25cbe9a3722f183991729e694d5978905c) |
| Dan Hipschman | 2008-04-09 | [qedit: Implement IMediaDet\_put\_Filename.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc3d6fbe7fcaf0d6c73817d4a600e8b3cba24038) |
| Dan Hipschman | 2008-04-09 | [qedit/tests: Fix an incorrect count given to GetTempPathW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=063aa3a1afb6c5441f76a13dc16e3fddf47ff99e) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Make the pullpin forward the BeginFlush before doing its own flushing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=994af69cac31bc53842ad13570bcce6797b89207) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Don't free a null media type in the file source.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4763e83b60528a8564332d3ba18c51d3e4509f6c) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Make the DirectSound renderer return S\_FALSE packet if in the paused...](http://source.winehq.org/git/wine.git?a=commitdiff;h=de117c1eb54488f839a790d5901ae34c3063dfd3) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Drop packets in the transform filter if in the wrong state.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8939a41563608585dbbfa0e76ce95237e93c3419) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Try creating the file reader from the filter source first before...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0117468754bdf53266b6ea752a44528abb744c67) |
| Maarten Lankhorst | 2008-04-09 | [quartz: Make mpeg splitter keep track of play position and keep last sample if...](http://source.winehq.org/git/wine.git?a=commitdiff;h=4bc4457109075bd25ab8a5bd4dc8101636074f56) |
| Maarten Lankhorst | 2008-04-08 | [quartz: Fix deadlocks in pullpin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4d9c09dd44d9ba32434787cee5f3a44fa54a899) |
| Maarten Lankhorst | 2008-04-08 | [quartz: Make wait timeout in directsound slightly larger.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1aa222e85938424bf85b95f395df5a13877b644) |
| Lei Zhang | 2008-04-08 | [user32: Handle VK\_ESCAPE correctly in EDIT\_WM\_KeyDown.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6736ed82ed5cb416771390c5c1bee7781e95b61c) |
| Lei Zhang | 2008-04-08 | [user32: Handle ES\_MULTILINE correctly for WM\_KEYDOWN/VK\_RETURN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f10fe07443a7eadb2b491981e69b1cbca9b5808) |
| Lei Zhang | 2008-04-08 | [user32: Fix WM\_CHAR return value for edit controls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8a4bb8fff225aa74d9a2c115cde7f2c4d31c5ba) |
| Lei Zhang | 2008-04-08 | [user32: Add tests for edit controls and VK\_TAB.](http://source.winehq.org/git/wine.git?a=commitdiff;h=42d32aba0223dcf4a08b577a2b32f7f65cc3faaa) |
| Lei Zhang | 2008-04-08 | [user32: Add tests for edit controls and VK\_RETURN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1abf27f8d3057131cf0bbc01bbfff121fdcb9c9) |
| Lei Zhang | 2008-04-08 | [user32: Add more tests for single line edit control inside a dialog.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e91de3952191b1a5775b00adb62d5ef320b3d01f) |
| Lei Zhang | 2008-04-08 | [user32: Add more tests for ES\_WANTRETURN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8cf7eef073955e825a675485234b7ef1d6f00cea) |
| Dmitry Timoshkov | 2008-04-07 | [winex11.drv: Do not set window type to utility to avoid a Metacity bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1bf824e0b00d2b179d5f34dd0c7ace83e83bd28a) |
| Alexandre Julliard | 2008-04-07 | [winex11: Don't set NET\_WM\_STATE on the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=334e88bc02305362c473ad362521f7801cdb86e4) |
| Jacek Caban | 2008-04-07 | [mshtml: Added IHTMLWindow2::get\_navigator implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c352a11cc4425053b58ea978e6931e9e1cb11cc) |
| Jacek Caban | 2008-04-07 | [jscript: Added IObjectSafety implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d95c210c891755cdc1c0eb0608c91ee2e108dec) |
| Dmitry Timoshkov | 2008-04-07 | [winex11: Change the priority of evaluated window styles to workaround a...](http://source.winehq.org/git/wine.git?a=commitdiff;h=751a71a0449e44a603894fa7e8b6dc27fb31c014) |
| Alexandre Julliard | 2008-04-07 | [winex11: Set the \_NET\_WM\_STATE atom directly for unmapped windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd97acbadffdc8af6d2682cb761a92ff2ab2f355) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Handle flushing and end of stream notifications for input pins.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01c6e64da67ffde47cd846d37d3f254f7cc56cc0) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Reset EcCompleteCount before starting filters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee792916e0b33de1f65499d01ff5f48416fd271d) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Fix past mistake to release lock during seeking and changing state.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d3dcc4e07d9046a71a49309003690859b73422e) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Fix some memory leaks in the file source.](http://source.winehq.org/git/wine.git?a=commitdiff;h=45bd38ece3ce8dda36ae1c3e8d5cac942b6013ef) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Make FileAsyncReader\_WaitForNext return an empty sample in flushing...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d56c50c85b96fbb13593c460572673e48c75b26a) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Get rid of code duplication and add a flush method.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fab66ee7a04e8b6072888c2c53502dafa0d7ad26) |
| Maarten Lankhorst | 2008-04-07 | [quartz: Add more state transitions to the filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f7c1d07527e4e9e2236fe6c7c9a5e0b12062403) |
| Maarten Lankhorst | 2008-04-07 | [dsound: Hold lock in GetStatus.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98933362f379e8a108703d9d5631f86e1c788fd1) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Add a partial test for IMediaDet\_get\_StreamMediaType.](http://source.winehq.org/git/wine.git?a=commitdiff;h=742120ba94b2b9d58a9a0d5bd3eaa2b84434d21e) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Add a test for IMediaDet\_(put|get)\_CurrentStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b37ee801668d67cbdac6b072d08bdf4c17f3698d) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Add a test for IMediaDet\_get\_Filename.](http://source.winehq.org/git/wine.git?a=commitdiff;h=07f9c44b36450e98ece1427843b3894a998febf0) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Add a test for IMediaDet\_get\_OutputStreams.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b0b47ac5f58f37bf06e76ab51173fd7617891774) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Add test framework and test for IMediaDet\_put\_Filename.](http://source.winehq.org/git/wine.git?a=commitdiff;h=999bc5bcb292a796454d081abf0ca1d868a00090) |
| Dan Hipschman | 2008-04-07 | [qedit/tests: Don't forget CoUninitialize.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b432b3655637aaf4541906def9ff301b9801731) |
| Michael Moss | 2008-04-07 | [wine.inf: Move winebrowser.exe to the system directory.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a8d26a9cf6da9fe0a05a26411fe81fa0bfae707) |
| Dan Hipschman | 2008-04-04 | [qedit: Indicate the methods of IMediaDet are not implemented in the FIXMEs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f95a849a28948549b0870f7c3a76cf5cf64638d6) |
| Lei Zhang | 2008-04-04 | [user32: Use a bogus wildcard in listbox test, change wildcard string to a const.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4bc0cd60cf87055b84b99d4e3e03fc7ddf7db5f7) |
| Maarten Lankhorst | 2008-04-03 | [user32: Implement BroadcastSystemMessage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70a6495a31cc01d6ea4284d4a6dadf037d9b60df) |
| Dan Hipschman | 2008-04-03 | [widl: Fix a mistake in an ordered list (keywords).](http://source.winehq.org/git/wine.git?a=commitdiff;h=976f570f61af5a7bf3aaf3102c7a7f5490f208e5) |
| Maarten Lankhorst | 2008-04-03 | [quartz: Fix memory leak found by valgrind.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cfeca053b843be495f356837b1dcfdf314717b0a) |
| Maarten Lankhorst | 2008-04-03 | [winemp3: Change a few more fprintf's to wine logs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5fdb793edd20abd152b50b90ebd2eb78492cdec) |
| Lei Zhang | 2008-04-03 | [user32: Correctly handle VK\_RETURN for edit controls with ES\_WANTRETURN style.](http://source.winehq.org/git/wine.git?a=commitdiff;h=376e45429cda0844b2106cc444a8cf7bac33de00) |
| Lei Zhang | 2008-04-03 | [user32: Dialog should ignore WM\_KEYDOWN messages if it gets DLGC\_WANTCHARS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08a4d2afc2ddfc1e508ef8528d5332d4b915b0a0) |
| Lei Zhang | 2008-04-03 | [user32: Add more edit dialog tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d1f1373af9b0210a09add13e2c7013cbe578b40) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Implement seeking on the null renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c0ea9eaa8ef3faacd27b759153a435739825418) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Fix stop\_playback used in pullpin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d6239bdace63b9148fb03b8c24965a4fa28b43e) |
| Alexandre Julliard | 2008-04-02 | [wineboot: Make services.exe inherit the wineboot event to keep it alive.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d478cc42d8e12d88f5165bff902adc28d0afe936) |
| Maarten Lankhorst | 2008-04-02 | [include: Add BroadcastSystemMessageEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4136355f01f4f550cbd09a2cff64e7f01e38f5b) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Make acmwrapper respond to a sample discontinuity by dropping the frame...](http://source.winehq.org/git/wine.git?a=commitdiff;h=975dc033024fb7f9215930a5bf75d38ac83dd481) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Add seeking to mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=553fe8565df83e3dc024841fdb2354ce088386cf) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Prepare mpeg splitter code for seeking by making most splitter parsing...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b1b75243d494da501f13c6cb213ff91255853ad0) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Fix parser and pins logic to no longer deadlock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e9ed6b402c6d7a49be736623d7e2bcf649d270b) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Implement filtergraph mediaseeking setposition.](http://source.winehq.org/git/wine.git?a=commitdiff;h=855e3a08b527f38bbc1b996982f6c8693c48b039) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Don't hold lock when changing state in filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7cb1324ae3d5924d8191d86ac2ab6306b2de36ad) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Fix locking in MediaSeeking and forward SetPosition.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b5d06d30f681c95743f5f80f7f898946611c9b4) |
| Maarten Lankhorst | 2008-04-02 | [quartz: Implement seeking stubs for transform filters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e18129068e3fcfdf98c8b8ee571d4ee015b13646) |
| Maarten Lankhorst | 2008-04-01 | [quartz: Implement graph MediaSeeking GetPositions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c56389ea3cd4ab211c5770b01530d7bd9b86df18) |
| Maarten Lankhorst | 2008-04-01 | [quartz: Small mpeg splitter fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6fd90f16259fd91743ca6bb7869c5e2d15a43f45) |
| Maarten Lankhorst | 2008-04-01 | [quartz: Allow parser filters to implement their own seeking methods.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1544e5239723522ede0054f033cf2067d9f59971) |
| Maarten Lankhorst | 2008-04-01 | [winemp3: Replace fprintf with wine debugging facilities.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0faee4af8504eef86a5b86b279a0afca4a1b32c3) |
| Rob Shearman | 2008-04-01 | [advapi32: Remove some unused services functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d834fc180df2d126334a98bc1f4ea245434ebae) |
| Rob Shearman | 2008-04-01 | [services: Fix memory leak of some data in the service record.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b7a37acdcb883eaaf83073aef01834261d14e1c) |
| Rob Shearman | 2008-04-01 | [rpcrt4: Add a reference to the binding object in I\_RpcNegotiateTransferSyntax...](http://source.winehq.org/git/wine.git?a=commitdiff;h=8aeb2858e44627c2002b9a20483a2a9c78a2aa3f) |
| Rob Shearman | 2008-04-01 | [rpcrt4: Improve trace in RPCRT4\_find\_interface to print the interface...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c7f9b9347fdf7a073329d9b3fada993c2ea74717) |
| Alexandre Julliard | 2008-04-01 | [ntdll: Add a guard page at the bottom of the stack and raise a stack overflow...](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc33f6c8a5df21589efa7ce26f8b13715e698008) |
| Alexandre Julliard | 2008-04-01 | [ntdll: Add support for handling page faults caused by guard pages on the thread...](http://source.winehq.org/git/wine.git?a=commitdiff;h=061bfac076b1c191b123f64f51579cc9ea8b68cc) |
| Alexandre Julliard | 2008-04-01 | [ntdll: Moved stack allocation for thread and process to a common routine in...](http://source.winehq.org/git/wine.git?a=commitdiff;h=600694546f6805c2e1a88a05e056a8b00d187d6e) |
| Jacek Caban | 2008-04-01 | [mshtml: Fixed copy&paste mistake.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d1cf6ce34b110defa122c4ac0c49a89ea8b60c9) |
| Jacek Caban | 2008-04-01 | [include: Added activedbg.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ab87d4dee37800b3f44a01dda66e430a7d0d92c) |
| Alexandre Julliard | 2008-03-31 | [wineboot: No longer needs to keep running now that we have services.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd2ee68d6d8bf8951f3227ae39b5fda4430522dd) |
| Dan Kegel | 2008-03-31 | [gdi32: Test retrieving BI\_BITFIELDS info for 16bpp modes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=338539c7090075918c5135df83366bb7058da537) |
| James Hawkins | 2008-03-31 | [fusion: Add initial tests for IAssemblyCache.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e021cff3d6af045b4d2e302f0a76054afdd0aa1) |
| Maarten Lankhorst | 2008-03-31 | [quartz: Check against a null dereference and don't read beyond the end of file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=714e807aa538681472719e038f2741f5bff69a7c) |
| Jacek Caban | 2008-03-31 | [mshtml: Added parsing external scripts support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cb7b58c528c874f40c4d47319de19cc20bab5b6e) |
| Jacek Caban | 2008-03-31 | [mshtml: Added parsing inline script support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=620a9500e25da9fdcda49a038869322ed8d29ec9) |
| Jacek Caban | 2008-03-31 | [mshtml: Return S\_OK in OnEnterScript and OnLeaveScript.](http://source.winehq.org/git/wine.git?a=commitdiff;h=40ab8e0c17feb4e41ce3f29d3bb8773428437c6e) |
| Jacek Caban | 2008-03-31 | [mshtml: Added IActiveScriptSite::GetItemInfo implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=438350321163d99497a667000e9f5358be4e54bf) |
| Jacek Caban | 2008-03-31 | [mshtml: Added IActiveScriptSite::GetLCID implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b24151b5df3b4dbfc055f402228657115b7edc54) |
| Jacek Caban | 2008-03-31 | [mshtml: Added IActiveScriptSiteWindow stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2db8f1a160e2b08e2e434097525de7497e063315) |
| Rob Shearman | 2008-03-29 | [services: Fill in the functions between implemented functions in svcctl.idl so...](http://source.winehq.org/git/wine.git?a=commitdiff;h=8529a3c404893ecbc710d4398cf43c6d1e36d650) |
| Rob Shearman | 2008-03-29 | [services: Introduce an scmdatabase object to store the root key of the services...](http://source.winehq.org/git/wine.git?a=commitdiff;h=809d714f243be1259b8b1553ee183c592620a3a9) |
| Rob Shearman | 2008-03-29 | [services: Remove dependency on service name being determined correctly in order...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8348b95a6accb18ae1df8d2c911f1b0bcf938fc) |
| Rob Shearman | 2008-03-29 | [services: Move ControlService and StartServiceW from advapi32.dll to...](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a6fc01d84f65e6ac3ba2bffad796ac655e99564) |
| Rob Shearman | 2008-03-29 | [services: Move LockServiceDatabase and UnlockServiceDatabase from advapi32.dll...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7afd9a977a84e80a02109351faa8d46182504c05) |
| Rob Shearman | 2008-03-29 | [services: Move SetServiceStatus and QueryServiceStatusEx to services.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b48714b14814dfbfda6606d608a51299a8a77eff) |
| Miko&#x0142;aj Zalewski | 2008-03-29 | [services: Move GetServiceDisplayName to services.exe and implement...](http://source.winehq.org/git/wine.git?a=commitdiff;h=010dcb168b434661c0ad91d47743e9bddb8c07e2) |
| Miko&#x0142;aj Zalewski | 2008-03-29 | [services: Move ChangeServiceConfigW implementation from advapi32.dll to...](http://source.winehq.org/git/wine.git?a=commitdiff;h=76d4eeebff5ee0fe6d56304cbcbe5294888b10a8) |
| Miko&#x0142;aj Zalewski | 2008-03-29 | [services: Move QueryServiceConfigW from advapi32.dll to services.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a363b9a066ab10e384f74fe5e9b438c3a1b36999) |
| Miko&#x0142;aj Zalewski | 2008-03-29 | [services: Move CreateService, OpenService and DeleteService implementations...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a2156fc348263c3fbd95c59b064746e8d74a21c4) |
| Miko&#x0142;aj Zalewski | 2008-03-29 | [services: Start a local RPC server.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4275fbf603d69e70ea0133e4b9abea44086812d1) |
| Jacek Caban | 2008-03-28 | [mshtml: Added IActiveScriptSiteInterruptPoll stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05935eb6b80fa6fc01acaf2f9857026726d9a82c) |
| Jacek Caban | 2008-03-28 | [mshtml: Set script engine state to SCRIPTSTATE\_CONNECTED when page is loaded.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac6cbb79afa01c85331c3317301e53285123814c) |
| Jacek Caban | 2008-03-28 | [mshtml: Added script engine initialization implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0db1b86c175c5055965986049b59914ebf1e03c9) |
| Jacek Caban | 2008-03-28 | [mshtml: Added IActiveScriptSite::OnStateChange implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d905ddd41a9fe2b2c87b93f16c5281e047a2a35) |
| Jacek Caban | 2008-03-28 | [uuid: Include objsafe.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d5bf9cd8ac7d5ca60ab52a9bb8ff1e26d84c876) |
| Maarten Lankhorst | 2008-03-28 | [quartz: Add GetCurrentPosition using the reference clock.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39623a403a99ee32ba3d16d2db316544dccb417e) |
| Maarten Lankhorst | 2008-03-28 | [quartz: Change name from Start position to Current position in MediaSeeking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc3ef90db000235f8de7a6692e9db79eda9680f3) |
| Dan Hipschman | 2008-03-28 | [wininet: InternetReadFileExA should check INTERNET\_FLAG\_ASYNC.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0929593b6c96a9dd482919b56f0a39d3ed015cb0) |
| Dan Hipschman | 2008-03-28 | [wininet: HttpSendRequestExA is not a stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aaecdf79bdb0fef0c04901dc03f4540ad62f3f11) |
| Lei Zhang | 2008-03-28 | [user32: Add more DrawText tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bab3d82bcf0df511d07d29b525b2614465d94f3b) |
| Lei Zhang | 2008-03-28 | [user32: Handle WM\_CHAR messages better in edit controls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0fac05b97791145cc624034733ab474169640156) |
| Lei Zhang | 2008-03-28 | [user32: Add more dialog with edit control tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d6bf737dbac8730b1ed229e88ec0a604239551e) |
| Lei Zhang | 2008-03-28 | [user32: Make an edit test more readable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1560203215f19a969c91564e99161876a52858a4) |
| Jacek Caban | 2008-03-27 | [mshtml: Don't access released object in release\_script\_hosts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7b48298e2755a18a7782aac87f06ce880e9c1e0a) |
| Dmitry Timoshkov | 2008-03-27 | [user32: Add a test for combobox navigation with arrow keys, make it pass under...](http://source.winehq.org/git/wine.git?a=commitdiff;h=113f2c9dbbf13517ebcfb5986b1f81a8fbede1db) |
| Jacek Caban | 2008-03-26 | [mshtml: Added nsIChannel::SetContentType implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e2645dec1cd3d9ad0b67a43db8112be8022f879b) |
| Jacek Caban | 2008-03-26 | [mshtml: Rename nsChannel::content to content\_type and clean up its handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8abf7a8cc94f43266f1246e1c9df52e19559ded0) |
| Jacek Caban | 2008-03-26 | [mshtml: Added IHTMLDocument2::get\_location implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1caf73be28dda1ad6fcc9ba3f2d0349686d300b7) |
| Dan Kegel | 2008-03-26 | [kernel32: Test negative dest len in WideCharToMultiByte.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dcefb67781e261aff504562f4902a00ceacc673f) |
| Alexandre Julliard | 2008-03-26 | [winex11: Fix X11DRV\_CLIPBOARD\_ReadProperty to read data in larger chunks and to...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a71998d0a60fb3c67aefe1938cc794f8263a7591) |
| Lei Zhang | 2008-03-26 | [user32: Tweak how the edit control handles WM\_GETDLGCODE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41ea8f0e8a6fab93fa08da16ecc24260dbad327c) |
| Lei Zhang | 2008-03-26 | [msxml3: Fix compiles for systems without libxml2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=724d4b1fad2a213044937f9b658065a35ad7d9c6) |
| Lei Zhang | 2008-03-25 | [comdlg32: Avoid double free in PRINTDLG\_PaperSizeA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19ed9729db3a73f0860ab621047cafc0a6b41c58) |
| James Hawkins | 2008-03-25 | [fusion: Implement CreateAssemblyCache.](http://source.winehq.org/git/wine.git?a=commitdiff;h=823640fc2faf80ef478989032ce631638ee30f15) |
| James Hawkins | 2008-03-25 | [fusion: Add a stub implementation of IAssemblyEnum.](http://source.winehq.org/git/wine.git?a=commitdiff;h=082b46887a548599f980c08a58f07d1789e76d67) |
| James Hawkins | 2008-03-25 | [fusion: Add a stub implementation of IAssemblyCache.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8a19faf261a23a54f6777b2acc94fce76f152e63) |
| Jacek Caban | 2008-03-25 | [mshtml: Added script engine loading test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d23309c040dc0e5e9da5983e67a6f91f8de08143) |
| Jacek Caban | 2008-03-25 | [mshtml: Added script engine loading implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1b5bce0d4c7e53ef0a151d2d916f99063c135d73) |
| Jacek Caban | 2008-03-25 | [jscript: Added tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63ebe0191e3881956b5bbd8308ef2b117f40533f) |
| Jacek Caban | 2008-03-25 | [jscript: Added DllCanUnloadNow implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d4aa7decf3c6b7cba9697a09dc3cc44dd71ae05) |
| Alexandre Julliard | 2008-03-24 | [user32: Make sure we set menu capture to a window that is visible.](http://source.winehq.org/git/wine.git?a=commitdiff;h=635544e20f52a939ed133fddba0d54f65baf2a2f) |
| Alexandre Julliard | 2008-03-24 | [winex11: Grab the pointer in menu tracking mode too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=78de7e363b8b9aeb0b7adb1083186da4ae58899a) |
| Alexandre Julliard | 2008-03-24 | [winex11: Setting window z-order using a sibling doesn't work with some window...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5787c12ba66c055bc0747ef63644df1dbfad86be) |
| James Hawkins | 2008-03-24 | [fusion: Add a stub implementation of IAssemblyName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b83fbb4f03176c651c7beaef8ebf75f2641ff9da) |
| James Hawkins | 2008-03-24 | [fusion: Add a few fusion stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=87b970cedcaa6e0403a651c9afff3a883a3188db) |
| Jacek Caban | 2008-03-24 | [mshtml: Abstract BSCallback implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8bb048b1a82d78b263542d5d217cb7e067a8758) |
| Jacek Caban | 2008-03-24 | [mshtml: Move hlink\_frame\_navigate function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6738db5af2dcdc4c61d9f20f9d889f8965537121) |
| Jacek Caban | 2008-03-24 | [mshtml: Move BSCallback declaration to navigate.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a7caae954015c45debc762934161e9211c765c71) |
| Jacek Caban | 2008-03-24 | [mshtml: Added new nsChannelBSC type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a04f526ad21ccf5bb4d3f323805172003cdaadf) |
| Jacek Caban | 2008-03-24 | [mshtml: Don't access BSCallback directly in nsembed.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=979b42d749d89f021bdc5554f542d27c47d5572a) |
| Jacek Caban | 2008-03-24 | [mshtml: Don't access BSCallback directly in nsio.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f792ada40fcbb755f09f3497277fa11adcf79233) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Silence requests for ipin on filters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db8b2ca7b49efdf9d021ed7c902ea70d4976f4dd) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Forward requests for MediaSeeking from all pins properly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4d745e0051e56de36deec70e3fbd80055733a7db) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Play silence in directsound renderer on end of stream notification.](http://source.winehq.org/git/wine.git?a=commitdiff;h=17a1c646869784f3cdeef1f976c35801b13f6f7d) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Make acmwrapper code aware of time, and get rid of its internal buffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8bb8384555c7d03376ad2af9bbc196f631ea89e) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Add sanity check to mediaseeking setrate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c423511d2ee5d3ece6c91286109c91030dfd258a) |
| Maarten Lankhorst | 2008-03-24 | [quartz: Parse audio packets in mpeg splitter to obtain the duration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b0c6a34358b5f2f9e1111f426dbeee4ef22a8d87) |
| Dan Hipschman | 2008-03-22 | [advapi32: Add a stub for CreateRestrictedToken.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2904f543f4593c5101b32b1044794f36d62bd7d5) |
| Jacek Caban | 2008-03-21 | [jscript: Added IObjectSafety stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cd0213bcb90f0315e676c8f1c81b61988558615a) |
| Jacek Caban | 2008-03-21 | [jscript: Added IActiveScriptParseProcedure2 stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0d8cbc6ef6b0ada17bd3e1001f0b0b336c348e2) |
| Jacek Caban | 2008-03-21 | [jscript: Added IActiveScriptParseProcedure2 declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96219452722091018a2d3c8fc469d01fe652841f) |
| Jacek Caban | 2008-03-21 | [wine.inf: Register jscript.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f460cbf9aff6a74e6def11fd294b0c236ae63e06) |
| James Hawkins | 2008-03-21 | [fusion: Add a stub implementation of fusion.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c0b3af34b999c7fca2e530b81d356ea9036d228d) |
| Dan Hipschman | 2008-03-21 | [widl: Make structures with FC\_ENUM16 fields complex.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2fa83d94c877233f4eaf1e8d8c17c7b74c3f9ec8) |
| Dan Hipschman | 2008-03-21 | [rpcrt4: Handle FC\_ENUM16.](http://source.winehq.org/git/wine.git?a=commitdiff;h=629a29d81e3611056bcf1a987e59b14399e5923f) |
| Michael Moss | 2008-03-20 | [kernel32/tests: Test notifications for overlapping directory watches.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ded68372a29eecc057718137a35f668f9d26d497) |
| Dmitry Timoshkov | 2008-03-20 | [user32: Increase an initial buffer size from 32 to 128 hwnds for enumerated...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0506c341ac3c51c6b1ccb1ecd65165e3b17a62dd) |
| Michael Moss | 2008-03-20 | [kernel32/tests: Fix false positive file notification tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef7c4a8b6daf783773a9ca0f29602d3afab13abf) |
| Lei Zhang | 2008-03-20 | [comctl32: Correct listview hittest check to include the state rect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74f2f09295175fdf813e2808eadd5934e18c71d2) |
| Lei Zhang | 2008-03-20 | [comctl32: Fix listview redraw when deleting items.](http://source.winehq.org/git/wine.git?a=commitdiff;h=03f18eb425b16ad5388018e8ed1d59061591c77f) |
| Lei Zhang | 2008-03-20 | [comctl32: Implement listview checkbox toggle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe966335fd7d808f6055649ee3796bf82eae566c) |
| Lei Zhang | 2008-03-20 | [comctl32: Redraw listview after changing extended styles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da98243ea13636a826bc94bf85853fd7bad62d50) |
| Lei Zhang | 2008-03-20 | [comctl32: Add listview checkbox toggle test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=778c04db079d3955bcea263bb5693c624318bf75) |
| Lei Zhang | 2008-03-20 | [comctl32: Add listview checkbox toggle test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=778c04db079d3955bcea263bb5693c624318bf75) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Transmit pullpin messages further.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea537b916e4a15fc39d9462445db9731f0849bec) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Implement forwarding mediaseeking messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e02322aef89dd3b452ff2e566692ad4d3bab5776) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Pass the reference time + small delay on on begin of playback.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d38b8502a6858e5d727385a7b06df3822c17a5dc) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Fix checking for duration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c53a803ab73c78519e97f4e8da9021b0576ebc15) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Add mediaseeking stub to audio renderer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ec4240065f1494fb90c2e1aa61be1330f9fe340) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Add critical sections to IMediaSeeking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=734d6159d520e8440e72d7518f22d250e639ff51) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Fix bug in transmitting messages further.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c9e2263eeedbe532ca6dbae58667c3238256bdc) |
| Maarten Lankhorst | 2008-03-20 | [quartz: Don't pass reference time when running.](http://source.winehq.org/git/wine.git?a=commitdiff;h=366eca51df96b9fa5c1f63cd93c4162b46151ce2) |
| Dan Hipschman | 2008-03-20 | [qmgr: Add a stub implementation of IBackgroundCopyJob2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d664c276dffc1f0f53ef6700ef182ef9c8c5d70c) |
| Dan Hipschman | 2008-03-20 | [rpcrt4: Use correct count in rpcrt4\_conn\_np\_write.](http://source.winehq.org/git/wine.git?a=commitdiff;h=764cf334d6aa909a29cf21e4d9a90ce06209598a) |
| Jacek Caban | 2008-03-19 | [jscript: Added IActiveScriptProperty stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ff3c3955d4dbe48d5160ae769c17a83f6c8f84b) |
| Jacek Caban | 2008-03-19 | [jscript: Added IActiveScriptParse stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12a589843607bd413086dea9596fa1b426e4a559) |
| Jacek Caban | 2008-03-19 | [activscp.idl: Added IActiveScriptProperty declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e553c56956470f9fe9f0413bc9a75273a16537a7) |
| Maarten Lankhorst | 2008-03-19 | [quartz: Move IMediaSeeking from the parser pin to the parser filter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=796bb9233322df53ea5c772c166484c7754ef822) |
| Maarten Lankhorst | 2008-03-19 | [quartz: Call send flush/endofstream and segment messages downstream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebf6bbd50f40bb0616607b27fa1040285841a5ed) |
| Dan Hipschman | 2008-03-19 | [widl: Ignore libraries in imported IDL files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d37b1a4969896d69d782b7ec55fc4e85690af0a7) |
| Maarten Lankhorst | 2008-03-19 | [quartz: Fix the magic bytes for mp3's with id3 tags.](http://source.winehq.org/git/wine.git?a=commitdiff;h=24708e4edb1c664b624505b15eb4df06a56e5036) |
| Maarten Lankhorst | 2008-03-19 | [winemp3: Skip idv3 header too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2756bedd8aa0a191f6d3d64d16cb41b8d6331303) |
| Dan Kegel | 2008-03-19 | [shell32: Only print &quot;HCR\_GetFolderAttributes should be called for simple...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5b499d37a8824b953e5cee9df674ef052a53ef8) |
| Alexandre Julliard | 2008-03-18 | [winex11: Clip out children window when repainting the desktop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af369106dbc9361c4329adb6e1b1cec3b2f7990b) |
| Alexandre Julliard | 2008-03-18 | [server: Fix desktop window coordinates mapping in expose\_window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2ea5723528e0e8a9336e0f4a5fd9e8a7fad0edb) |
| Maarten Lankhorst | 2008-03-18 | [wine.inf: Change default windows version to XP.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f629dc4eb6006fbdc3f658d13186b9c7e08b189d) |
| Maarten Lankhorst | 2008-03-18 | [winmm: Fix midi deadlock by not holding lock on release.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15907b5035ea7f03b369a0463ab1f6ac2b24704e) |
| Maarten Lankhorst | 2008-03-17 | [dsound: Add an option to mix sound buffers in the mixer again.](http://source.winehq.org/git/wine.git?a=commitdiff;h=021019ff8fbc49a778abcf7800edacb4fa33068d) |
| Jacek Caban | 2008-03-17 | [jscript: Added JScript stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0750bfbb1d5f9c470b5554e35c9c324f9bbe7015) |
| Jacek Caban | 2008-03-17 | [jscript: Added JScript class factory.](http://source.winehq.org/git/wine.git?a=commitdiff;h=85b024d5f71195b815d51ab990fdde02f6b66bed) |
| Maarten Lankhorst | 2008-03-15 | [user32: Fix enumeration for EnumWindowStations and EnumDesktops.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd69ababec3b26e76837ed0d3cd82509c619a38e) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Implement a few MediaSeeking functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f8b16f117207a1f9e41963cb732cca44b492ab3) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Change some more stubs from traces to fixmes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=18f42a6eb70678aef06cd10a5a8d7139f614c996) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Add initial support for time formats in IMediaSeeking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b662a6a556c8144cf7586d5f17b92f59b9dce3c4) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Make MediaSeeking stubs fixmes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ffe48d40137003f59cb5a6df053ea1384a51e414) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Silence the directsound buffer on starting.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d965b8fb6cbb892662e5324155e6c5b2efb430d) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Set a default sync source on the filtergraph.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b1f9acc68862d28a934f5fa5a6e2ec2635af9df6) |
| Dan Hipschman | 2008-03-15 | [qmgr: Implement IBackgroundCopyJob\_AddFileSet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=136a4ebbb2237994c1289b35685d62666c50a66a) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Destroy the filtergraph better in releasing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d47bdbfbf166884a1fd93fd97a628dd418a18e97) |
| Maarten Lankhorst | 2008-03-15 | [quartz: Fix IFilterGraph RemoveFilter to stop the filter before removing it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14ba79ec621bf60855016297cded61cc865daf5a) |
| Jacek Caban | 2008-03-14 | [urlmon: Added special URLACTION\_SCRIPT\_OVERRIDE\_SAFETY handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ef6713acb5e3287c1b0c6ce6ff27485a427f482) |
| Jacek Caban | 2008-03-14 | [urlmon: Added more policy tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a736c6677cecf588368c44314390ebff239df72) |
| Jacek Caban | 2008-03-14 | [urlmon: Added ProcessUrlAction implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15feb50d424a4cd017d1e4dacfc5c4302c24a550) |
| Jacek Caban | 2008-03-14 | [urlmon: Added URLACTION\_\* and URLPOLICY\_\* declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19b6cf8135e74bde820b669f248efacda221fbe2) |
| Jacek Caban | 2008-03-14 | [urlmon: Fixed URLZONEREG\_DEFAULT handling in GetZoneActionPolicy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfb1089a45f17c596fdcf86ebcda8acfced6259b) |
| Jacek Caban | 2008-03-14 | [mshtml: Return full patch in res protocol's secure URL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f7748b9b577397ac874f3479874ae95c55bf62a) |
| Jacek Caban | 2008-03-14 | [urlmon: Move InternetParseUrl(PARSE\_SECURITY\_URL) call to map\_url\_to\_zone and...](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc159d832deea4e0a4a5d28b9c8152d4be848637) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Add directsound renderer to filter list.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c09284c9193e74aaa6a047ca651f366351fdf99) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Implement detection on file extension in filesource.](http://source.winehq.org/git/wine.git?a=commitdiff;h=25f9d3c17366b6454dba49b2897304c2248137fe) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Uncomment a trace.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83efc64dd505ffb91aeaad39ec90850ef0c322fe) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b5a8df58cba34730cf475d5bd988fff6e116423b) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Detect and skip id3v2 header in mpeg splitter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c1d089a44c8a31037566b56979bca5ec3daaba6) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Implement a dummy null renderer for directshow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e1867dac0d82cd3fcede46f3bb08e5d8875865f6) |
| Maarten Lankhorst | 2008-03-14 | [quartz: Don't add MERIT\_DO\_NOT\_USE filters automatically to create a connection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=07b12032d2e9bd24bdf952df875e82449898857a) |
| Maarten Lankhorst | 2008-03-14 | [qcap: Implement a stubby CaptureGraphBuilder2::RenderStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=950d3443e768550062f2d0ca506b4d6ee00367cd) |
| Maarten Lankhorst | 2008-03-14 | [qcap: Add better findpin stub for CaptureGraphBuilder.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e32b11ab6ec2a53f70e6bf19144c04680011f1a) |
| Dan Hipschman | 2008-03-14 | [qmgr: Implement progress updates for downloads given by URL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9617b326182ab01e7b286b7a0e0fd4d0bcb8eebc) |
| Dan Hipschman | 2008-03-14 | [qmgr: Transfer files given by URL (including HTTP, etc).](http://source.winehq.org/git/wine.git?a=commitdiff;h=8199e3dfa261b65cfeab039939c0ab28bbbc5f3e) |
| Dan Hipschman | 2008-03-14 | [qmgr: Transfer files given by URL (including HTTP, etc).](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f2b3303d75a516877c88319f83a9a680464fe72) |
| Dan Hipschman | 2008-03-14 | [qmgr: Implement BackgroundCopyJob\_Complete.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1c93ee77e5cdf4e1fececbf576908889bcbe80dc) |
| Dan Hipschman | 2008-03-14 | [kernel32: Add the MOVEFILE\_WRITE\_THROUGH flag for MoveFileEx (stub).](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e8f1931846669818787255867397c415f5afd86) |
| Dan Hipschman | 2008-03-14 | [qmgr: Implement local file background &quot;downloads.&quot;](http://source.winehq.org/git/wine.git?a=commitdiff;h=b329a2ef3cdb17f4b301adcbe5beddf57506ace6) |
| Dan Hipschman | 2008-03-14 | [qmgr: Add infrastructure for background file transferring.](http://source.winehq.org/git/wine.git?a=commitdiff;h=374fea0a71cd7f141f491ec0abee9b5f14168d4a) |
| Dan Kegel | 2008-03-13 | [wintab: Expand whitelist of tablets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e4d5d21fd2236cba706bfe24a853a17e34de1cd) |
| Dan Hipschman | 2008-03-13 | [qmgr: Add critical sections for jobs and files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd499df4d5dca5aff2cd179b2149bafbcd3b81d1) |
| Jacek Caban | 2008-03-12 | [jscript: Added Dll[Un[](http://source.winehq.org/git/wine.git?a=commitdiff;h=66c728dec1a37f10c6e039f0a63558c05590ab9d)]RegisterServer implementation.] |
| Alexandre Julliard | 2008-03-12 | [user32: Add a SetCapture function to the driver interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b9dee8efa7e74c49169cedf53788fefb69c3b1a5) |
| Alexandre Julliard | 2008-03-12 | [user32: Add a helper function to set the capture window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e129f88d0e8e212702a33906d3ce9609837f4f5) |
| Lei Zhang | 2008-03-12 | [shell32: Use xdg well known directories for desktop folder symbolic link.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8cbd8bd87e85d07f1d134a712b1c452c90fc3a0) |
| Lei Zhang | 2008-03-12 | [shell32: Use xdg well known directories for my\_xxx folder symbolic links.](http://source.winehq.org/git/wine.git?a=commitdiff;h=78f5db2b511cb8b558f1198dbf640781e929de8f) |
| Lei Zhang | 2008-03-12 | [shell32: Add xdg-user-dirs lookup code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5ba1c21bea6a66455a478910575fcad9c9024a4) |
| Lei Zhang | 2008-03-12 | [comctl32: Fix TB\_GETSTRING return values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f5c97693e2301918d16577578c237dd81852a14) |
| Lei Zhang | 2008-03-12 | [comctl32: Add tests for TB\_GETSTRING, fix NULL pointer access.](http://source.winehq.org/git/wine.git?a=commitdiff;h=375f60b07af4fec5d16bb5534f52379b61811053) |
| Alexandre Julliard | 2008-03-11 | [winex11: Discard ConfigureNotify events even if the intervening events are for...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e874fded991d85c30f4d4f5d728923a5ff96a1ee) |
| Jacek Caban | 2008-03-11 | [include: Added activaut.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe5ea9f006ada0a79ba2fad2cb82d476ea3393d1) |
| Jacek Caban | 2008-03-11 | [activscp.idl: Added CATID\_\* declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7ba25f0b22698d5ebc48d1c02400c1c2268540c5) |
| Alexandre Julliard | 2008-03-11 | [winex11: Add support for merging redundant events, and use it for...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0118e0d0f10fb61abcfeb5100b206b94594d4493) |
| Maarten Lankhorst | 2008-03-10 | [include: Add flag for BSM\_ALLDESKTOPS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=619ac152d5479f3c6ad035e0eecaf4e6a16cf26d) |
| Jacek Caban | 2008-03-10 | [jscript: Added stub DLL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa23a2c4b68ce2dd5d506075099949d3e476d78d) |
| Jacek Caban | 2008-03-10 | [urlmon: Fixed MapUrlToZone test on IE7.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bbfae3deffcb395bc068ff5111f682c3cc09b584) |
| Dan Hipschman | 2008-03-07 | [qmgr: Only have one BackgroundCopyManager per system.](http://source.winehq.org/git/wine.git?a=commitdiff;h=275f00f54d29682729d2286e2ddf8a5f0c74d6e1) |
| Maarten Lankhorst | 2008-03-07 | [server: Fix reference leak in enum\_desktop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b164ce484e388e4e78fe16c658e52daec749367) |
| Dan Kegel | 2008-03-07 | [winex11: wintab.c: use atan2 instead of atan.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1eba6c7644f801f82c66b109f39d754f0c4e05f2) |
| Lei Zhang | 2008-03-06 | [quartz: Validate input for FilterGraph2\_AddFilter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0831be5adcf440b6ffb8b68c75d0f65df1e7290f) |
| Maarten Lankhorst | 2008-03-06 | [include: Add flag for BROADCAST\_QUERY\_DENY.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8d8ddab110a89d2ad7a3bf5d7f33b1ed58306d0) |
| Maarten Lankhorst | 2008-03-05 | [oleaut32: Handle TKIND\_ALIAS properly when passed as pointer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c978bbee87dd6e09e4ad836df5ad7d63506face2) |
| Dan Hipschman | 2008-03-05 | [qmgr: Implement IBackgroundCopyJob\_Resume.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb7043699341d0bbf861529d6e07a557e990a298) |
| Lei Zhang | 2008-03-05 | [shell32: Remove unused variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5637c779d24fbecd609cf5288f5d650cb25f3d8c) |
| Roy Shea | 2008-03-04 | [qmgr: Implement IBackgroundCopyJob\_GetProgress.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc484a9b934d3abbd1e360f4b0af1990c791c464) |
| Roy Shea | 2008-03-04 | [qmgr: Implement Skip and Reset for IEnumBackgroundCopyJobs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0fd05f09ec7f7aef41be809285ae6aba30047e4) |
| Roy Shea | 2008-03-04 | [qmgr: Implement IEnumBackgroundCopyJobs\_GetCount.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8dfba77c8cfcf235ee2c6b8927059c8b97f9ac0b) |
| Dan Hipschman | 2008-03-04 | [qmgr: Implement IEnumBackgroundCopyJobs\_Next.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1317e3115adc0e580a333602ae1f27f89730c6a8) |
| Alexandre Julliard | 2008-03-01 | [winex11: Set the appropriate \_NET\_WM\_STATE properties for maximized windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9238ccca487620a96ddbfb9d203fb50b460601e5) |
| Maarten Lankhorst | 2008-03-01 | [kernel32: Fix GetVolumeInformation for fat32 partitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1032ba6dc3aca18365152ecd10b428deda5c3e83) |
| Maarten Lankhorst | 2008-03-01 | [cfgmgr32: Forward some more functions to setupapi.](http://source.winehq.org/git/wine.git?a=commitdiff;h=109943cc4c3889fb90b8c9dc2f94bd66e27cb46f) |
| Maarten Lankhorst | 2008-03-01 | [setupapi: Implement CM\_Get\_Device\_ID and add a stub for CM\_Get\_Parent.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba8642639aa8f682c0b6441b6636d2322c204206) |
| Roy Shea | 2008-02-29 | [qmgr: Implement job lists for IBackgroundCopyManager.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8a0e98b719cbb072a1ee8503761d8547dfca671) |
| Roy Shea | 2008-02-29 | [qmgr: Implement IBackgroundCopyFile\_GetProgress.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e6cbde105f81990bb96c5b243e78ba77582f28ba) |
| Roy Shea | 2008-02-29 | [qmgr: Implement GetLocalName and GetRemoteName for IBackgroundCopyFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4866d1bde66848f550ca39ba2686e052bcfc126f) |
| Roy Shea | 2008-02-29 | [qmgr: Implement Skip and Reset for IEnumBackgroundCopyFiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c4776c2a343c08615249f3c898d2c7f37a969f4) |
| Dan Hipschman | 2008-02-29 | [qmgr: Implement IEnumBackgroundCopyFiles\_Next.](http://source.winehq.org/git/wine.git?a=commitdiff;h=980e00c63b17906413fe99c54b897001d1f63630) |
| Roy Shea | 2008-02-28 | [qmgr: Implement IEnumBackgroundCopyFiles\_GetCount.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84a5eca28e660174cc4a1a4fe443fdb084945941) |
| Roy Shea | 2008-02-28 | [qmgr: Implement IBackgroundCopyJob\_EnumFiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=27421285b9d8bf578fb3b8df5316409a2d0238a5) |
| Alexandre Julliard | 2008-02-27 | [winex11: Check the current window state on Map/UnmapNotify and ignore obsolete...](http://source.winehq.org/git/wine.git?a=commitdiff;h=eaea28e5d83b8d302eed62dbf574b5d6d2c14cdd) |
| Alexandre Julliard | 2008-02-27 | [winex11: Added tracking of the WM\_STATE window property.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a5344b4ad2b9be527940c8d259961e4b4e9cfb8) |
| Alexandre Julliard | 2008-02-27 | [winex11: Clear the NET\_WM\_STATE status when a window is withdrawn.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9939b7b4305def8505aa16b631ba6d76d74def53) |
| Roy Shea | 2008-02-27 | [qmgr: Implement IBackgroundCopyJob\_AddFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be8bac15fd43756aeaac883c145c17645729dc90) |
| Roy Shea | 2008-02-27 | [qmgr: Implement the IUnknown interface for IEnumBackgroundCopyFiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83aee6b1a30a29d2b8e7052c3a2cc1c48cb29faa) |
| Roy Shea | 2008-02-27 | [qmgr: Implement the IUnknown interface for IBackgroundCopyFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=128654ba0805eb132d77f2e3963694f25b9b8c0d) |
| Dmitry Timoshkov | 2008-02-27 | [kernel32: Return upper cased drive letters in paths, some applications depend...](http://source.winehq.org/git/wine.git?a=commitdiff;h=aebcbf0f6e10d80b04bc4a3dcd3e8ca55dfd60d0) |
| Maarten Lankhorst | 2008-02-27 | [shlwapi: Don't add a trailing slash in the case that nothing has to be appended...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b254b407a494633127c3977a27794b958c776174) |
| Maarten Lankhorst | 2008-02-27 | [wininet: Fix retrieving raw headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5132fb4469a4914f6459486d69280b0745e11808) |
| Roy Shea | 2008-02-26 | [qmgr: Implement IBackgroundCopyManager\_EnumJobs with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9f63253d001055d6e95c18f1e4ebed136e545c10) |
| Roy Shea | 2008-02-26 | [qmgr: Implement the IUnknown interface for IEnumBackgroundCopyJobs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00a3dceb75ccccc9589af81ac92be25ac21e6bf3) |
| Roy Shea | 2008-02-26 | [qmgr: Implement IBackgroundCopyJob\_GetDisplayName with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=28e7c3b9a93afc0010b5c498e098a49ced458156) |
| Roy Shea | 2008-02-26 | [qmgr: Implement IBackgroundCopyJob\_GetType with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f126b4a60ab7dde5d772147e23c7302df70f434) |
| Maarten Lankhorst | 2008-02-26 | [wininet: Add stub for INTERNET\_OPTION\_PER\_CONNECTION.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60401737c61520ccf57779be2cbeed49beea25b5) |
| Roy Shea | 2008-02-25 | [qmgr: Implement IBackgroundCopyJob\_GetId with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=575b1bfcc7919966064fc3ef2fe29e14b89c456b) |
| Roy Shea | 2008-02-25 | [qmgr: Implement IBackgroundCopyManager\_CreateJob with test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=111e6929ac9067694efd55c710c7609e1d988522) |
| Roy Shea | 2008-02-25 | [qmgr: Implement the IUnknown interface for IBackgroundCopyJob and stubs for the...](http://source.winehq.org/git/wine.git?a=commitdiff;h=fee94bbc9e4098930822bb62317ea1bf1685fa06) |
| Dan Hipschman | 2008-02-22 | [widl: Allow is\_string\_type to work for typedef'd types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d7b1f18b16759a820589c6cf21d64ee19a63da5) |
| Maarten Lankhorst | 2008-02-22 | [advapi: Check if service really exists before bombing out in CreateService.](http://source.winehq.org/git/wine.git?a=commitdiff;h=284f86183cce638ff8fce4023cb76273e979aa09) |
| Alexandre Julliard | 2008-02-21 | [winex11: Make the BitBlt short-cuts more generic to apply to all possible ROPs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23afe2e94cc3321331f6e8e0bb4556afbd242e50) |
| Dmitry Timoshkov | 2008-02-21 | [winex11.drv: Add an optimized path for BitBlt(SRCINVERT).](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae8457e431f9733415ae6a183c275dce3dd30826) |
| Alexandre Julliard | 2008-02-20 | [user32: Pass the modified SetWindowPos flags to the set\_window\_pos server...](http://source.winehq.org/git/wine.git?a=commitdiff;h=55165f87cce88e6b49f2436ef0f9d7dc12e25285) |
| Dmitry Timoshkov | 2008-02-20 | [user32: Add a z-order test for owned popup windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9f23c3f9d5cba98117dadca03cb68145a01539f8) |
| Roy Shea | 2008-02-19 | [qmgr: Add some tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=884e7e7b5661a398e0ce36a585f5b6698517ffb5) |
| Roy Shea | 2008-02-19 | [qmgr: Add ServiceMain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c51ad2c3f78cf801b7458a810c4490f85421ed1) |
| Roy Shea | 2008-02-19 | [qmgr: Implement DLL server registration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=313a903a8503ff674eb18a7514012c0f56117ca9) |
| Lei Zhang | 2008-02-19 | [qedit: Add stub implementation of MediaDet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4868cde91d34d493c67b60ed28e9ef25a0edc177) |
| Lei Zhang | 2008-02-19 | [qedit: Add tests directory and a simple test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8551a073db54c4a58363b180bf02def20bfe018) |
| Lei Zhang | 2008-02-19 | [qedit: Add MediaDet registration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4f7a5c5c952de127c8cc367dfe45fafbe922175) |
| Lei Zhang | 2008-02-19 | [include: Add IMediaDet interface and MediaDet class.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e2ce6982968a65464aa216a2ba5818781331fd4) |
| Lei Zhang | 2008-02-19 | [include: Add ISampleGrabber interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=121e8ebbbe9ad5e408f5ee39711b419f67713d72) |
| Lei Zhang | 2008-02-19 | [include: Generate qedit.h, add ISampleGrabberCB interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a69b83f1eedb72d3851c151014a80863fffb317) |
| Lei Zhang | 2008-02-19 | [qedit: Add the DirectShow ClassFactory.](http://source.winehq.org/git/wine.git?a=commitdiff;h=080c0812bc310203d1885328758a53427b7063b3) |
| Lei Zhang | 2008-02-19 | [qedit: Skeleton implementation of qedit.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6de8be71b3b849ab2c510829977ee7f6c33d359c) |
| Maarten Lankhorst | 2008-02-18 | [dssenh: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2472e81cea2854d0dd2f491f88852c6667ead9c9) |
| Maarten Lankhorst | 2008-02-18 | [softpub: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e11826f553158d880c7c922f97a0267e5bb7f881) |
| Maarten Lankhorst | 2008-02-18 | [slbcsp: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b3a9699ab3e3f60d135b2b80f73fb8ba2540ec6d) |
| Maarten Lankhorst | 2008-02-18 | [sccbase: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=322d4cab1e6b1c6ddbb9be86d6e0ffef2aeab1d4) |
| Maarten Lankhorst | 2008-02-18 | [mssip32: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c438d23902824e077a5c26f3c76971a060edec5d) |
| Maarten Lankhorst | 2008-02-18 | [initpki: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c3d24bf5cdec69f5ef7432925d1d8053562e12a) |
| Maarten Lankhorst | 2008-02-18 | [gpkcsp: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4576c807ba771c2d5cb63edec58eb6330ebb51c) |
| Maarten Lankhorst | 2008-02-18 | [cryptdlg: Add initial stub dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9308217792c47ccda45e462107a89dbed126be2) |
| Alexandre Julliard | 2008-02-18 | [user32: Rewrite SWP\_DoOwnedPopups to take into account topmost windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f15dd4d4e4424a84623f4af7c71b955e7aa234b) |
| Maarten Lankhorst | 2008-02-18 | [user32: Fix a message test that would only pass on wine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c6e61fbf892fe80bd34dfedeff3eaeeec43d0236) |
| Maarten Lankhorst | 2008-02-16 | [browseui: Add undocumented Component Category Cache Daemon stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a33ab3484e8b12f426448cedc6104d5db988a9bf) |
| Maarten Lankhorst | 2008-02-16 | [include: Add IRunnableTask interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e07112ba5bce86aa6ed0001f9b16b0032cbae5d3) |
| Dmitry Timoshkov | 2008-02-15 | [user32: Use custom window procs instead of DefWindowProcA/W in the...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d421a47834ba2328bf609c709886e487a0736b3) |
| Dmitry Timoshkov | 2008-02-12 | [user32: Add a couple of tests for WS\_EX\_TOPMOST.](http://source.winehq.org/git/wine.git?a=commitdiff;h=066c60eb312609737b4b66e69c91750612364b05) |
| Dan Kegel | 2008-02-12 | [msvcrt: Fix EOF behavior on read from pipe or console.](http://source.winehq.org/git/wine.git?a=commitdiff;h=316869b273ce8bbed968d6380c1b89f07187090a) |
| Lei Zhang | 2008-02-08 | [quartz: Add VideoRendererDefault.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9742724afeed8a03c19b9dac3eaa995ad557ac8e) |
| Lei Zhang | 2008-02-07 | [user32: Use wine\_dbgstr\_rect() in traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c1cdc71869ba175e30730ebbc6a86cef5ff89d7) |
| Lei Zhang | 2008-02-07 | [comctl32: Use wine\_dbgstr\_rect() in traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=398040123177368fc37dd20345dd3888a29a5b93) |
| Dan Hipschman | 2008-01-24 | [oleaut32: Use the symbolic name for TYPEFLAG\_FDISPATCHABLE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0820c1840f7a7bcf367c325c118ed85a4109546) |
| Alexandre Julliard | 2008-01-24 | [winex11: Check for need to make window managed when WS\_VISIBLE is set outside...](http://source.winehq.org/git/wine.git?a=commitdiff;h=8913182b89d542633678d1c3abcfe00e28be8e6d) |
| Alexandre Julliard | 2008-01-23 | [user32: Menus should be top-most windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a753f90cf61be5ed6d93d336b1ace01e9ca75b1) |
| Alexandre Julliard | 2008-01-23 | [comctl32: Tooltips should be top-most windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e85f7ed79ea6e74674d92136a0cbb084aafd133f) |
| Alexandre Julliard | 2008-01-23 | [winex11: Export a function to dock a window into the system tray, and get rid...](http://source.winehq.org/git/wine.git?a=commitdiff;h=cbdf1294e6474ae5254a2fe9cb900b08a89b8b1b) |
| Roy Shea | 2008-01-23 | [qmgr: Implement IClassFactory methods.](http://source.winehq.org/git/wine.git?a=commitdiff;h=807fc8c5433770e2ebc1d5f06e495eb998da0515) |
| Lei Zhang | 2008-01-23 | [ddraw: Register the DirectDraw 7 Object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8bbb3d68e1772531796e4c209d4d7ba85da9b997) |
| Alexandre Julliard | 2008-01-22 | [server: Invalidate the correct region when custom valid rects are specified.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2921f5c156b368b4ce6e615eb61dad5c5f423bf8) |
| Alexandre Julliard | 2008-01-16 | [winebuild: Don't try to use the .init section on Mac OS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aaf02c6f4a6105f8186b5e6b1c3179e80f213c88) |
| Alexandre Julliard | 2008-01-16 | [wineboot: Delay import the dlls that are not needed for the default initialisation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c06ba6fd8e3845e3b92239168a529c2f4b0e96d) |
| Alexandre Julliard | 2008-01-16 | [ntdll: Fall back to a server device ioctl for files with no associated fd.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b71d645f05d9728ab28c8f3be5709a5fd5365f1) |
| Alexandre Julliard | 2008-01-16 | [winebuild: Reserve the space for the PE header in the .init section.](http://source.winehq.org/git/wine.git?a=commitdiff;h=538071ce7e8052ea317950bb13615f09af315911) |
| Alexandre Julliard | 2008-01-16 | [mountmgr.sys: Fix values returned for IOCTL\_STORAGE\_GET\_DEVICE\_NUMBER on emulated ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=4003457ff3b328295b40ce43d8c68f0e0250b889) |
| Alexandre Julliard | 2008-01-16 | [wineboot: Add a --init option used when launched automatically at startup.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d6d080d4b2dc0afbc65e3b64c8f13086dfdce48) |
| Alexandre Julliard | 2008-01-14 | [kernel32: Don't inherit stdin/stdout handles in wineboot.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c00a78da52dc14acdb391ae02ec10a63d3b85ab) |
| Alexandre Julliard | 2008-01-14 | [user32: Don't inherit stdin/stdout handles in explorer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7687f78f7133fc0891e0b76f097415f77dc10411) |
| Alexandre Julliard | 2008-01-14 | [kernel32: Close the stdio handles when creating a detached process.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a3132343d9c6f1b87f79034d80ef6595e4a1bbd) |
| Alexandre Julliard | 2008-01-09 | [mountmgr.sys: Implemented IOCTL\_DISK\_GET\_DRIVE\_GEOMETRY and IOCTL\_STORAGE\_GET\_DEVICE ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1796650353a8094d2496eb102ef873ec47071ee) |
| Alexandre Julliard | 2008-01-07 | [wineboot: Don't print errors for non-fatal problems.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebac63e17c4768f4f284752ac3fecf2b9030cbcf) |
| Alexandre Julliard | 2008-01-07 | [kernel32: Fail more gracefully in GetVolumeInformation for fake drive devices.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c486d8774f9c1e9849b42d22e69d98be71596a36) |
| Alexandre Julliard | 2008-01-07 | [advapi32: Fix the length written to the pipe for the start message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=781c3b9c6aebacd869a026993f8ae84be2159de1) |
| Alexandre Julliard | 2008-01-07 | [ntdll: Return a proper Information field also when opening a server file object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44dbb07441202aa0be0ca864984d428dc3d77492) |
| Alexandre Julliard | 2008-01-07 | [server: Wait for the expiration of all the process SIGKILL timers before exiting ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f1e73cb3576bf4e7b065dacca06c3196f8591ad) |
| Alexandre Julliard | 2008-01-04 | [kernel32: Launch wineboot on first startup of a wine process.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d55b2de5747da90666065b5ed2fdeb8049282419) |
| Alexandre Julliard | 2008-01-04 | [kernel32/tests: Added tests for FindFirstVolume/FindNextVolume.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d17b29303cd9075123033f159339f9872c14b227) |
| Alexandre Julliard | 2008-01-04 | [mountmgr.sys: Implemented the IOCTL\_MOUNTMGR\_QUERY\_POINTS request.](http://source.winehq.org/git/wine.git?a=commitdiff;h=838f12539bf54370d0c344d8b6d880ac303ffb39) |
| Alexandre Julliard | 2008-01-04 | [kernel32: Implemented FindFirstVolume/FindNextVolume using the mount point manager.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f508df25b1e068f58e8299dd113f51b014c721e) |
| Alexandre Julliard | 2008-01-04 | [mountmgr.sys: Add devices to the MountedDevices registry key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6befc98dba09aae816692da159be4fb3431b2a57) |
| Alexandre Julliard | 2008-01-04 | [mountmgr.sys: Added initial stub for the mount point manager device.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43dc80e623d00781c726892ef0eddce7b03c9db7) |
| Alexandre Julliard | 2008-01-04 | [advapi32: Don't wait for 20 seconds if a service fails to start.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3133280d08538ac68b4d49aeecc1327f2eb15ddc) |
| Alexandre Julliard | 2008-01-04 | [mountmgr.sys: Create disk devices for all configured drives.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2143dee78a0acf8be8c07062e84cc12ef18ef7cb) |
| Alexandre Julliard | 2008-01-04 | [mountmgr.sys: Create a hard disk device for PhysicalDrive0.](http://source.winehq.org/git/wine.git?a=commitdiff;h=07e92a7dad0c881efda10b5f3c914c178b0bbcf9) |
| Alexandre Julliard | 2008-01-02 | [server: Redesign the server shutdown processing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af268c621131624fc34f34ccab9fcd8d47500c31) |
| Alexandre Julliard | 2008-01-02 | [server: Use exponential backoff when waiting for wineserver -k to complete.](http://source.winehq.org/git/wine.git?a=commitdiff;h=307cb09a62072ccf2b24df9a1be8a5f3b5e44e47) |
| Jeremy White | 2007-12-31 | [wintab32: If we could not find a stylus sort of device, we haven't found a tablet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=659494660e77c4fbe0186f92fab3724d02d1619e) |
| Jeremy White | 2007-12-31 | [wintab32: Add logic to detect specific tablet cursor types, use it to discard non ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=51aecf8056748b4a9abcf67ec8f5dc7c73f76af2) |
| Jeremy White | 2007-12-30 | [wintab32: Add modest trace information for tablets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca89d7e80998a817b4ed82e30901854b3f70cf8a) |
| Jeremy White | 2007-12-30 | [wintab32: Remove the unused and clearly broken FindOpenContext function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c1d38649ae547d57dbb91bc07281390d0b3befa) |
| Lei Zhang | 2007-12-28 | [gdiplus: Initialize a variable in a test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b810430f1fe5777cfe5f71e69c7478623346ad8b) |
| Lei Zhang | 2007-12-28 | [gdiplus: Add GdipCreatePen2 and test cases.](http://source.winehq.org/git/wine.git?a=commitdiff;h=003b5de4f2f08bf1d278ef0dd05cd6004f621afb) |
| Jeremy White | 2007-12-24 | [wintab32: Don't return information for non existent cursors.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5adac3b1960ed2803e27346b799eafbe98bc99a) |
| Jeremy White | 2007-12-24 | [wintab32: Capture the number of buttons earlier, allowing our button maps to be fille ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f193197a66c052c81d006e4c7ab40247ef7f0411) |
| Maarten Lankhorst | 2007-12-24 | [winealsa: Add special case for microphone source in mixer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7034b92d904baa71f1bc885d0078d8ab6ae47f35) |
| Jeremy White | 2007-12-24 | [wintab32: Fix the W-&gt;A translation for CSR\_NAME and CSR\_BTNNAMES.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51ea5cb4e8e314ff2712ac13fbac0e820de3ca51) |
| Jeremy White | 2007-12-24 | [wintab32: Implement the ability to return the number of devices and cursors.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3036e7f626dac9e5728029a5951f2d538bf6ccd4) |
| Jeremy White | 2007-12-24 | [wintab32: Add constants for cursor types and use them.](http://source.winehq.org/git/wine.git?a=commitdiff;h=047a969658f1efe7fa3bea7b4c713d123f63ac70) |
| Jeremy White | 2007-12-23 | [wintab32: Do not offset the physical device id by the cursor number.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee0554b737b817c3009e33e764f976464590809f) |
| Jeremy White | 2007-12-23 | [wintab32: Compute our physical device characteristics based on the first tablet devic ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d58429d085cdf890d9362a30b36626ca419e5b5a) |
| Jeremy White | 2007-12-23 | [wintab32: Store and use the physical device id to match device to cursor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c9fcb15b11773c5d37d0bf5546dffe7939d8596a) |
| Jeremy White | 2007-12-23 | [wintab32: Correctly handle devices with a device id of 0.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9267fcd99fb54d58b0928734a7ffe41fc479a4f3) |
| Jeremy White | 2007-12-23 | [wintab32: Order the cursor array by the standard Wacom promulgates.](http://source.winehq.org/git/wine.git?a=commitdiff;h=64a929c48353b68cc4cd177d37ed25308abf282b) |
| Jeremy White | 2007-12-23 | [wintab32: Add additional device tracing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5132ab4693edfad9704d0dd223778c6e6ad86e80) |
| Alexandre Julliard | 2007-12-23 | [kernel32: Initialize MaximumLength of the user params directory too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=28aed6d9c886cd566d27e9aff162203be2ad0959) |
| Alexandre Julliard | 2007-12-21 | [kernel32: Store the initial directory as a full path in the process parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4269c8eed130acd3a767ca36da80265e0340a8a) |
| Lei Zhang | 2007-12-21 | [quartz: Make filtergraph aggregatable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99a193ce7e661abb23b2a3ff982d8afc5eacd2ee) |
| Lei Zhang | 2007-12-21 | [quartz: Move aggregation tests into separate file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ddb13381eac3b73bc2e9e6b0db4d0f60799c280) |
| Alexandre Julliard | 2007-12-20 | [server: Don't count system processes as users of a desktop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ffbeae78f76f4b6c1ce2d51093473044b9f49522) |
| Alexandre Julliard | 2007-12-20 | [advapi32: Move the EnumDependentServicesA/W stubs in service.c where they belong.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb2d8458a371bbfab81a125814ccafebd82e16d9) |
| Alexandre Julliard | 2007-12-20 | [wineboot: Rewrite wininit.ini processing to use GetPrivateProfileSectionW. Convert ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e34244a3b9c7cb0be4de3c24c99d8de82b5d3815) |
| Alexandre Julliard | 2007-12-20 | [include: Added the mountmgr.h header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1b356745b1fae791e9977154eaff06b5c639b00) |
| Alexandre Julliard | 2007-12-20 | [explorer: It no longer needs to be made a system process.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a32873bfcc3f0e96cb7853797d3930668720a93a) |
| Alexandre Julliard | 2007-12-20 | [wineboot: Add support for starting NT-style services.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f6e1db3e0c40bd99035605149d08f54af3f694e) |
| Alexandre Julliard | 2007-12-20 | [advapi32: Start non-interactive services in a separate window station.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7593fac6327bc8e95848801c83ae00cfee547c54) |
| Roy Shea | 2007-12-20 | [qmgr: AddRef, QueryInterface, and stub functions for queue manager interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=702e6d8d152557f5107f1b55e7ae31cccf8b9441) |
| Alexandre Julliard | 2007-12-20 | [wineboot: Convert the rest of the code to Unicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a58b2847c50a3695e8a9fd4df70fbad7872b9e3) |
| Alexandre Julliard | 2007-12-20 | [server: Don't give out full access to the system process event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11750af32961f69da96cc04712f71cb4fc285383) |
| Alexandre Julliard | 2007-12-20 | [wine.inf: Mark the spool service as disabled, it's just a stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b85eee2363bcca934489e15a000b146bb683cf4) |
| Alexandre Julliard | 2007-12-20 | [wineboot: Simplify the unnecessarily complex code structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06e888f244a6bb548017f05f03bc4b8418f53e47) |
| Alexandre Julliard | 2007-12-19 | [advapi32: Return from StartServiceCtrlDispatcher when all services are stopped.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c673b2284d03c17154ccc977203cbc6d05a95e69) |
| Alexandre Julliard | 2007-12-19 | [advapi32: Replace the list of services with an array.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a12b9c52da5617d58c7c80823946287679b43452) |
| Alexandre Julliard | 2007-12-19 | [advapi32: Reimplement RegisterServiceCtrlHandler on top of RegisterServiceCtrlHandlerEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=865bb0a67a06720c94e1360c5ae4c669b364d60d) |
| Alexandre Julliard | 2007-12-19 | [advapi32: Fix RegisterServiceCtrlHandler spec entry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4889a0edf7a798928a297fb7b1e25f445e839eb6) |
| Alexandre Julliard | 2007-12-19 | [advapi32: Use exponential backoff when waiting for a service to start.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f11ad82886aa14d4aae6b9a7c04ad416a9dcb98) |
| Dmitry Timoshkov | 2007-12-19 | [user32: Set the edit text in a combobox only if combobox has strings.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e799c6d7bfefcce10323680ecd249286046cce4) |
| Alexandre Julliard | 2007-12-18 | [server: Fix possible NULL dereference.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c69468ddcc4478e29645372edd370a9ad353cea1) |
| Alexandre Julliard | 2007-12-18 | [ntoskrnl.exe: Added implementation for IoCreateDriver and IoDeleteDriver.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7ac931acf29dbf80ffbb27fed51c46bbd4bf3504) |
| Alexandre Julliard | 2007-12-18 | [ntoskrnl.exe: Allow returning data in ioctls along with a positive non-zero status.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f5131e47ffc366c2b99d247ffb7035e798af245) |
| Maarten Lankhorst | 2007-12-17 | [riched20: Fix bugs in EM\_SETOPTIONS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e639ec392b1652edd4a0f121e534f036b4ceac9) |
| Roy Shea | 2007-12-17 | [qmgr: Generate C file with local GUID definitions from bits.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ceb8e1f31fe3d6067c5ac201449e29409f5cc7f) |
| Maarten Lankhorst | 2007-12-14 | [riched20: Implement ECO/EM SELECTIONBAR.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b81335501f32fb11b3634faf7a5c484c458dabc8) |
| Maarten Lankhorst | 2007-12-14 | [winealsa: Add 'Front Mic' as alias for microphone.](http://source.winehq.org/git/wine.git?a=commitdiff;h=483e3be2e662616e79deade581d4ecb22333daf2) |
| Maarten Lankhorst | 2007-12-14 | [riched20: Make some functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4637a4ef49b56dfb3bbe7a3bebb26160e0e30e20) |
| Lei Zhang | 2007-12-13 | [quartz: Fix typo in GraphConfig\_AddRef.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5cd582bae61a8e1d7866eb16c48b8397976af59) |
| Lei Zhang | 2007-12-13 | [quartz: Set \*ppvObject to NULL if QueryInterface fails.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5075f73564c0956a22fa4f914da7187d91410c2) |
| Lei Zhang | 2007-12-13 | [quartz: Do aggregation test for more video renderer interfaces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8f69b5a427d571ba4850bde918064d56557b139) |
| Alexandre Julliard | 2007-12-13 | [user32: Print the RegisterHotKey fixme only once.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e533e50d59cea7c464641d49f7d2d7f918a5d923) |
| Lei Zhang | 2007-12-13 | [ole32: Print a fixme when an aggregation attempt fails.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5e78c84c70d3c525f4a26fb04ee4ee66f547770) |
| Lei Zhang | 2007-12-13 | [quartz: Make aggregation test generic.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf20ca1dd476d5647447e7983ff2ddf3c9ae7812) |
| Lei Zhang | 2007-12-13 | [quartz: Make video renderer aggregatable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=932cc2d7f910ec9a7df17384610832922e67b861) |
| Lei Zhang | 2007-12-13 | [quartz: Add videorenderer aggregation test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=766046d4ab5ad649bbf2203b573319b8e8667478) |
| Lei Zhang | 2007-12-13 | [quartz: Give video renderer's Inner\_QueryInterface a less generic name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63df94ba0b62d859c50b49969a3c6483fd62c57b) |
| Lei Zhang | 2007-12-13 | [quartz: Add videorenderer QueryInterface test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f6f1bcb6e82b3d53c084797ac5ba3d4967c3046) |
| Lei Zhang | 2007-12-13 | [quartz: Add referenceclock QueryInterface test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29cc256b9a92e91258a0df69a6c09f3a3641ac01) |
| Maarten Lankhorst | 2007-12-13 | [include: Update oleacc with new constants and IAccessible interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1733875f013c0c14e91bb916971247dbd26a67ae) |
| Maarten Lankhorst | 2007-12-12 | [winealsa: Add control 'Digital' as alias for microphone.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f75600dd1de81e016a44dee37391bc5bb051c7b6) |
| Alexandre Julliard | 2007-12-12 | [winecrt0: DriverEntry is a WINAPI function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6012061292e1dc2ebbf929736dd2244ae85fd3a) |
| Maarten Lankhorst | 2007-12-12 | [winealsa: Don't require a cswitch control for capture.](http://source.winehq.org/git/wine.git?a=commitdiff;h=affd447db0c7cb9c4c056916ce930d0ffd9511aa) |
| Maarten Lankhorst | 2007-12-12 | [winealsa: Remove fixed fixme.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e87f3741b758ab810e3ea966f21ea2344c59672) |
| Alexandru Balut | 2007-12-12 | [wine.inf: Fix the type of some values in HKLM, System\CurrentControlSet\Control\Sessi ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=586970365736da41cfac8d9cfc85b38962c91202) |
| Lei Zhang | 2007-12-11 | [quartz: Add IFilterGraph2 interface and stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cff265950a9c9e3e684ff99747800987851426de) |
| Alexandre Julliard | 2007-12-11 | [winebuild: Don't set the IMAGE\_FILE\_DLL flag on native modules.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b462c20876feae7b1384a50a8acfa5b376562bda) |
| Alexandre Julliard | 2007-12-11 | [Makedll.rules: Add a generic EXTRADLLFLAGS variable instead of defining a specific ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5fb981acea5ce23d134ea5fbb5f79d274783a19) |
| Roy Shea | 2007-12-09 | [qmgrprxy: Queue manager proxy generated using an IDL compiler and bits.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00ef4e5829305f77b5eafb796a07de84eb92877c) |
| Alexandre Julliard | 2007-12-08 | [kernel32: Read label and serial from the filesystem when the device is accessible ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5d63b55352f85a56e63dc0aaf5f74084de1403a) |
| Alexandre Julliard | 2007-12-08 | [kernel32: Revert change that slipped in commit db24d3af9a6e56c3036ba0a3e5d62dae4f2676 ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a3dd1ecf9571da6fd22a8bcb5b8f571e22481be) |
| Maarten Lankhorst | 2007-12-07 | [winealsa: Fix return value checking in wavein.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9fb2cacd64dd6a039b9edd4fbdf72c27a8bd6590) |
| Maarten Lankhorst | 2007-12-07 | [winealsa: Simplify the feeding of capture buffers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5290f53193d0d43ad2867098228a2599422ebf61) |
| Maarten Lankhorst | 2007-12-07 | [winealsa: Clear dwBytesRecorded in waveheader when adding buffer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=322cd0b9796ed2ed7c70f7298c90980bbe064f4a) |
| Maarten Lankhorst | 2007-12-07 | [winealsa: Fix period size in capture.](http://source.winehq.org/git/wine.git?a=commitdiff;h=02e1ce0a4236f80cc1782c78290a2b97f9caf5bd) |
| Lei Zhang | 2007-12-06 | [quartz: Move current tests into their own test case.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f84f4cab70b330daf3cfb0a1f2367b14d17d99a3) |
| Roy Shea | 2007-12-06 | [qmgr: Renamed bits\_main.c to qmgr\_main.c and updated comments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b655da64122ea7bb80dc44a4d602598bb39a5fe2) |
| Roy Shea | 2007-12-06 | [include: Added IDL file for BITS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a63f3e6a11925baec514f45b3ab660ad5c544156) |
| Roy Shea | 2007-12-06 | [include: Added bitsmsg.h header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68b55594a07b6a2ba47ed98b0799968e1cfb9681) |
| Lei Zhang | 2007-12-06 | [quartz: Add some IGraphBuilder related tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=646eefaa476995c387f8616a401c4dba6e2fccc8) |
| Lei Zhang | 2007-12-06 | [quartz: Add a test for IFilterGraph2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ab6fd3de0180bcd4acee4fc4b03f355a41a625c) |
| Lei Zhang | 2007-12-06 | [quartz: Fix return value in IFilterGraph\_FindFilterByName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31aab429340ac5c65adea83b769b36121507ba41) |
| Lei Zhang | 2007-12-06 | [quartz: Validate input for IFilterGraph\_FindFilterByName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d1a6016c9b18fabeb38a6dbe2fcfe82847706d1) |
| Alexandre Julliard | 2007-12-05 | [server: Implemented EnumWindowStations and EnumDesktops.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d30b5742edbd48d8687bdb17a9776bc6ad5e7d1e) |
| Alexandre Julliard | 2007-12-05 | [server: Partial implementation of NtQueryDirectoryObject.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5e38b332df0417e748f461a6946c0dad5cd293d) |
| Alexandre Julliard | 2007-12-05 | [server: Return correct object types in the get\_directory\_entry request.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8382eb01b2f2ed05a0a8131618e8c68e6581ad2d) |
| Roy Shea | 2007-12-04 | [wininet: Added check of dwStructSize required by Windows in calls to InternetCrackUrlA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91d07f699590d0a64f0f72e49e438db17f699c30) |
| Roy Shea | 2007-12-04 | [wininet: Removed inline from copy\_compsA and zero\_compsA to allow Windows testing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7903d7f3f480a1c571122f40ebd69a876a79bfdc) |
| Roy Shea | 2007-12-04 | [svchost: Implementation of svchost.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4714c4fa806280dc8a4f06e5e4bf5cda73ca6db1) |
| Alexandru Balut | 2007-12-02 | [oleaut32: Implement VarWeekdayName + tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90d8741d23c9cc19f7f9d285efea2c7f8467af1a) |
| Lei Zhang | 2007-11-20 | [shell32: Perform copy in UnixFolder\_ISFHelper\_CopyItems.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa057686bb52b0f39d4acc790c7d9b4b0f7f20e3) |
| Lei Zhang | 2007-11-20 | [shell32: Only notify immediate parent.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cb99cd331d34762dd093829e7d5e1b2be41a48af) |
| Alexandre Julliard | 2007-11-13 | [shell32: Don't wait for the command to terminate in ShellLink\_InvokeCommand.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db500aad2d65497e9a8e41d96345de7469dc7c15) |
| Alexandre Julliard | 2007-11-13 | [include: Added definition for SEE\_MASK\_NOASYNC.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74572e43bec5110423da4362603389ebc0be3884) |
| Alexandre Julliard | 2007-11-13 | [shell32: Pass some of the ShellExecute flags through InvokeCommand.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14eb294a484989daedf60ff598f9593f12416c8c) |
| Lei Zhang | 2007-11-12 | [shell32: rename My Video to My Videos.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70c75dcd0d7d39b67547e9700eec52dfd5dbc6d0) |
| Alexandre Julliard | 2007-11-12 | [user32: Remove a few traces that only duplicate the relay information.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ff78347e2ef1f0028eff30c3a4fca47c159a166) |
| Lei Zhang | 2007-11-12 | [shell32: Don't crash if $HOME is not set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4dda7c6371f04d6aaf8c7d37e58139a2acaee567) |
| Dan Kegel | 2007-11-11 | [advapi32: Fix buffer overrun in tests/registry.c:wine\_debugstr\_wn().](http://source.winehq.org/git/wine.git?a=commitdiff;h=89b9af77147cfc5afdb90bafb81228cd9bc4399e) |
| Lei Zhang | 2007-11-09 | [sane.ds: Get number of options only once.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e984d7ba40e6d7e6de78a2cd4f88f0b3a2f4f087) |
| Dan Kegel | 2007-11-09 | [user32: Implement return value for DdeClientTransaction for XTYP\_EXECUTE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aaa93200ad4f4880456fad0f4582e2e57695861f) |
| Lei Zhang | 2007-11-09 | [sane.ds: Check return value from sane\_get\_option\_descriptor().](http://source.winehq.org/git/wine.git?a=commitdiff;h=84e8ea2fdcba6ea76f023e8bd584a78896066e83) |
| Lei Zhang | 2007-11-09 | [wininet: Skip strcmp() in a test if the returned value/len is wrong.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83a4dbaa689d54f12ce05011c9f41b7637f3b75b) |
| Lei Zhang | 2007-11-09 | [sane.ds: Fix a memory leak.](http://source.winehq.org/git/wine.git?a=commitdiff;h=124f2aa27e45f4d6fe780ab172010fa27d8aa5cd) |
| Lei Zhang | 2007-11-09 | [sane.ds: Check return value from sane\_control\_option().](http://source.winehq.org/git/wine.git?a=commitdiff;h=05907c3e29aed2684bf3879cd28ae2b47e8c29c9) |
| Lei Zhang | 2007-11-08 | [wininet: Initialize ftp sockets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f727e56d6d330b5ed5103f4d93d25d529c792bfb) |
| Alexandre Julliard | 2007-11-07 | [include: Add WINGDIAPI to the exported gdi32 functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=caf56765d5b8294dc5fd1e51e7492c0fcc2559e6) |
| Alexandre Julliard | 2007-11-07 | [user32: Make all internal user32 functions and variables hidden.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c57b5057dbb3e27d3672ff2d50d19fbf98c0cfa5) |
| Alexandre Julliard | 2007-11-07 | [winebuild: Add a few nops to stub entry points to make Safedisc happy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c32e02e48d3aeba7588b566973c9fb02253e8a10) |
| Dan Kegel | 2007-11-07 | [msvcrt: Fix two buglets in heap test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1e4758f076190dbef7d06f9e10241d0aabe3788) |
| Alexandre Julliard | 2007-11-07 | [gdi32: Make all internal gdi functions hidden.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a368cc4756a5bd3ca6fe9380062bec95732a82d) |
| Alexandre Julliard | 2007-11-07 | [include: Mark imported functions with hidden visibility.](http://source.winehq.org/git/wine.git?a=commitdiff;h=95c728551d5ee9b71d2a6328d0220a8b678c5225) |
| Alexandre Julliard | 2007-11-07 | [include: Add WINUSERAPI to the exported user32 functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=919e32c034b6a9634b9d8101164c44d0548200e9) |
| Alexandre Julliard | 2007-11-07 | [include: Add NTSYSAPI to the exported ntdll functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6cf2df5a0c38472faa1081e477fb626079174e4f) |
| Alexandre Julliard | 2007-11-07 | [include: Only use DECLSPEC\_IMPORT for Windows compilers in unicode.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6678c07f5784365fee9dc3c43f71f9712897cfde) |
| Alexandre Julliard | 2007-11-07 | [include: Add WINADVAPI to the exported advapi32 functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d1da3430c2481e61f030475c24894a4df97b2bf) |
| Alexandre Julliard | 2007-11-07 | [include: Add WINBASEAPI to the exported kernel32 functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16d85e2d303e5612c575ab0fd1fd51542d670506) |
| Dan Hipschman | 2007-11-06 | [widl: Don't rely on type\_memsize to return 0 for all conformant arrays.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0ac63961d4b43e67a5aa2b58092f717d2c90ec7) |
| Jacek Caban | 2007-11-04 | [mshtml: Added AcceptLanguage handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3717bff1855f5c6a1c5ecbfae137dfb9deaf968) |
| Nigel Liang | 2007-11-04 | [wininet: Release object in HttpSendRequestExW before return on error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f44627b047674552ccaf61e666a3f4fc4b87cf7) |
| Dan Kegel | 2007-11-04 | [cabinet: FCICreate: Initialize oldCCAB.](http://source.winehq.org/git/wine.git?a=commitdiff;h=559b38c34ce9e43e623be74c344800ad45159264) |
| Dan Kegel | 2007-11-03 | [cabinet: FCIAddFile: Set defaults in case callback doesn't set some fields.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2330178eba94ea96db8a1bb03f2a34cc93290b5) |
| Dan Hipschman | 2007-11-02 | [rpcrt4/tests: Initialize memory in the get\_name test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eaffc0a0da2b1fbf6074235749eada78956e2f39) |
| Lei Zhang | 2007-11-02 | [comctl32: Fix uninitialized, unused variables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf313ee857b9167cb26b39040d6184f50b36c18f) |
| Dan Hipschman | 2007-11-02 | [widl: Don't output a void conformance for NdrClearOutParameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b0bc8e58def27bdf7d4c376fba3b091a0420d448) |
| Dan Hipschman | 2007-11-02 | [widl: Handle pointers to conformant arrays (e.g., &quot;[size\_is(, n)](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d15820f7934551a66005bf9c9ec1e5eaaf01742) int p; &quot;).] |
| Dan Hipschman | 2007-11-02 | [rpcrt4: Initialize allocated pointers to NULL in PointerUnmarshall.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8caa325eb7e5225a042622d8f8199adb1aa488a1) |
| Lei Zhang | 2007-11-02 | [comctl32: Fix typo in rebar.](http://source.winehq.org/git/wine.git?a=commitdiff;h=019016f90fcbef28059df3376ff425caad1b691b) |
| Lei Zhang | 2007-11-01 | [comctl32: Datetime should close its monthcal when the monthcal loses focus.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d05f7fc74294e1e4f72fe0e1cbeb0aae204f904) |
| Dan Hipschman | 2007-10-31 | [widl: Add a --local-stubs option.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea7ab4da66c4eb96768fc210e34e1e2d14e284a3) |
| Dan Kegel | 2007-10-31 | [ntdll: NtAccessCheck: Only send used bytes to server.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ab07d61b916cbdb698879226cc77075c4405ee88) |
| Lei Zhang | 2007-10-30 | [comctl32: Set tab focus correctly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2519fdcda334167b44899e188f3d9400a83ea13) |
| Alexandre Julliard | 2007-10-30 | [server: Remove failed ioctls from the queue as soon as the result is set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8268ad551a258de88f4e0338a19e4866fc0deea0) |
| Lei Zhang | 2007-10-30 | [comctl32: Add tab delete item / get focus test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=73213d14440d42e58fe1acc0ac1fc94dc14d32c5) |
| Lei Zhang | 2007-10-30 | [comctl32: Add tab insert item / get focus test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31a09c3b7bc0b89e59c77a1f361c095536046fe9) |
| Dan Kegel | 2007-10-29 | [advapi32/tests: Fix undefined memory references in registry.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc072e209d3016ed87adcf7f81adca17a706b56a) |
| Lei Zhang | 2007-10-29 | [comctl32: Move tab test's createParentWindow() into START\_TEST().](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5a17f98df43d5cac9b666334c9135479b7d935d) |
| Dan Hipschman | 2007-10-26 | [widl: Fix ExprEvalRoutines output.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70e12b31b8d4976fe4cdfc2dd74329e86d1a8170) |
| Dan Hipschman | 2007-10-25 | [widl: Allow void pointers with iid\_is attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f974facf5a7a04e27462ab83f3109fa50abec537) |
| Dan Hipschman | 2007-10-25 | [oleaut32: Use widl to generate oaidl\_p.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d7b34c19225e962af46cd6ad382de8103988d22) |
| Dan Hipschman | 2007-10-25 | [widl: Fix a crash in compare\_expr.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9825ac7a1a0e2ac0088efe6ffda30000a9da2dfd) |
| Lei Zhang | 2007-10-25 | [user32: Do not send button click to dialog with disabled default button.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c2263ddc4c6326d79a9d7f246eeba7ca7d45c5f) |
| Dan Kegel | 2007-10-25 | [winmm: Avoid testing linecontrols if can't get line info.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d9b69f5a32ee0778fa337c6471fe4b8fda8c3dd) |
| Dan Kegel | 2007-10-25 | [wine.inf: Add fake DLL for mshtml.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=374db6371ca0cd17fea47685489ad6cb99b475b5) |
| Dan Hipschman | 2007-10-24 | [widl: parser\_error must append a newline, so write a new function, error\_loc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9051918976a9fdd7b0dd6c09f5b5028d7b2a6616) |
| Dan Hipschman | 2007-10-24 | [oleaut32: Add stubs for IPropertyBag\_Read.](http://source.winehq.org/git/wine.git?a=commitdiff;h=816f99328827cc1d8e0885c4399a8e65ee56e69b) |
| Roy Shea | 2007-10-24 | [include/rpc.h: Add missing headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=79e7e15f25bfbd97e1532a69bdc1f642b91ae2c0) |
| Dan Hipschman | 2007-10-24 | [widl: Use error\_loc instead of yyerror.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1aab1072c1838d0f167dd94dc4c0c16ae9df5be3) |
| Dan Kegel | 2007-10-23 | [gdi32/tests: Fix false pass in warn+heap case.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4b0cf5f5b5b35beb40ec1cc4a4e6669729a38be) |
| Miko&#x0142;aj Zalewski | 2007-10-21 | [advapi32: Make CreateWellKnownSid create domain sids (with test).](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf509c29f121e908609ec36a984839f3e0186ff0) |
| Miko&#x0142;aj Zalewski | 2007-10-21 | [advapi32: Add a test for CreateWellKnownSid and implement two more SIDs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b06379b2b3afb3382d3ff50c8a71f566aef91f13) |
| Miko&#x0142;aj Zalewski | 2007-10-21 | [advapi32/tests: Define OBJECT\_BASIC\_INFORMATION in source file as it is not defined ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=8bc12f3f41004a71542155eea5947a296b6b695b) |
| Miko&#x0142;aj Zalewski | 2007-10-21 | [advapi32/tests: Make the SDDL test pass under Vista.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05cb54fcc86c98b0f79f58788d0c0562b8c18d7a) |
| Dan Hipschman | 2007-10-20 | [widl: Update the manpage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd6a276f4c93adcc3afe02a0e190b2454a13ef46) |
| Dan Hipschman | 2007-10-19 | [widl: Fix problems with variable-size user types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff8930f2bfdfd5a16924422fcd9e2730593952fa) |
| Alexandre Julliard | 2007-10-18 | [shell32: Check for internal shell classes before querying the registry in SHCoCreateI ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7892ccf2b5c702f59c01142249926ad6fd14324) |
| Alexandre Julliard | 2007-10-18 | [ntdll: Cache the DOS drives stat info for up to one second.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7fd1ad5ffaed038dd046dbdffdd2a66e5e6c6e67) |
| Alexandre Julliard | 2007-10-18 | [shell32: Use wine\_get\_dos\_file\_name instead of duplicating knowledge about the drive ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f092818f057ce02d0f8c4628cbf7e93c1d69040) |
| Nigel Liang | 2007-10-18 | [wininet: Release object in HttpEndRequestW after use.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d2ac2039b3212b1a2b6dccdda3fc0640787a696) |
| Dan Hipschman | 2007-10-18 | [widl: Improve file cleanup when errors occur.](http://source.winehq.org/git/wine.git?a=commitdiff;h=67c634c2035bcf4ddefddac4dc4bc7fc72b22923) |
| Dan Hipschman | 2007-10-18 | [widl: Remove printf format strings that aren't really format strings.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fb7a0e40ed9c8ef47faa1d4ce4f26a545614dcb) |
| Dan Hipschman | 2007-10-18 | [widl: Generate dlldata files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=40e90aae25198e7a059520c0258eefe3e817fe00) |
| Dan Hipschman | 2007-10-18 | [widl: Detect conformant arrays of user types correctly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d0f9378bc855652bf45db0e29b07fa85724dbd1) |
| Alexandre Julliard | 2007-10-17 | [winex11: Process all types of messages while moving/resizing a window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7fa032d1a4d34b0cb41add32235d122b10bd2734) |
| Dan Hipschman | 2007-10-16 | [widl: Use new functions need\_proxy and need\_stub to clean up code and avoid generatin ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f173addbef6759a5782023a5ac5da843e0b790fa) |
| Dan Hipschman | 2007-10-16 | [widl: Output the correct value for TableSize in ProxyFileInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebfbec6e5c29db673d00eaf16ce14981b950b312) |
| Dmitry Timoshkov | 2007-10-16 | [wordpad: Refuse to load OLE compound storage files like Windows does.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6b8ee0e41f0333de11cf837b21fba580a641c0f6) |
| Dmitry Timoshkov | 2007-10-16 | [user32: Add more listbox message tests, make them pass under Wine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=566ce8f5edd314d31a2f76f10da51d8674a66112) |
| Lei Zhang | 2007-10-15 | [comctl32: Select today's date when the today link is clicked.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e58e4679b5c745f4d4c450088fe617d28306ea3c) |
| Lei Zhang | 2007-10-15 | [comctl32: Monthcal should send notifications when today link gets clicked.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d81b6fa8c765926fd13977e2ff5bd65115432914) |
| Lei Zhang | 2007-10-15 | [comctl32: Correct monthcal WM\_LBUTTONDOWN return values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=76949d377838e0fabe553b321043226eca65c21f) |
| Lei Zhang | 2007-10-15 | [comctl32: Monthcal today link test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=734600e272efddb9153df425269814e2ae4a2cf9) |
| Lei Zhang | 2007-10-14 | [comctl32: Simplify monthcal test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3accf13ec0882ca66820d00c77f9892ae6cd0d17) |
| Dan Hipschman | 2007-10-12 | [rpcrt4/tests: Free memory from one of the tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e219087c65c3a4877e8e15941443cc9b3748d82b) |
| Nigel Liang | 2007-10-11 | [include/winsock.h: Fix parenthesis mismatch.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c31faf499156a631fedcc30015d94adb6a3d1617) |
| Dan Hipschman | 2007-10-10 | [rpcrt4, widl: Make pointer layouts compatible with windows; fix conformant array ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=acfde97b9ee3bd0df8d3bfc4a83ab538eb08b535) |
| Dan Hipschman | 2007-10-08 | [widl: Allow quoted UUIDs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cfa54572707404bfabe89ccd522ed8e6f00fb0db) |
| Roy Shea | 2007-10-08 | [qmgr: Skeleton implementation of Background Intelligent Transfer Service (BITS).](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b0255f6d8aacff0b2b68028508a5da041b78dd0) |
| Dan Hipschman | 2007-10-08 | [widl: Implement pointer\_default functionality.](http://source.winehq.org/git/wine.git?a=commitdiff;h=24ce74e96a49db7007a2e86399e9481d9a81e95f) |
| Dan Hipschman | 2007-10-08 | [widl: Keep track of every allocated type\_t to simplify set\_all\_tfswrite.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2226ddcadfeaf2029f67838bc5dc73094c8df366) |
| Lei Zhang | 2007-10-07 | [comctl32: Fix monthcal hit tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b8ca91d036f3e0098023abce4c992466ce4517d) |
| Dan Kegel | 2007-10-06 | [quartz: Make clock test less flaky.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e8f8401599dd49247b62294a77e3fe969ec8b8a) |
| Dan Hipschman | 2007-10-05 | [rpcrt4/tests: Make server.idl compatible with MIDL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e0b209815ddd31c95de8f4b5e6fd06cd0f28e858) |
| Dan Hipschman | 2007-10-05 | [widl: Make structs containing user types bogus; fix square\_test\_us test failure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d00ff2ed58a0ca17354fcc3072fede626821e6fb) |
| Dan Kegel | 2007-10-05 | [msvcrt: Fix ^Z handling in text mode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=56eb6f67305ae390c709adddd114fd9040334135) |
| Dan Kegel | 2007-10-05 | [msvcrt: Improve CR CR LF handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4cd3a16f181b30ffa0a1099d6d676c413b25cc22) |
| Dan Hipschman | 2007-10-03 | [widl: Correct default pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9650cf9bdbc5eb3aa37f932c51a4e039cce17b08) |
| Dan Hipschman | 2007-10-03 | [widl: Add newlines to error messages that are missing them.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c8c425f425907ddb6abf33294000e76e940ca05) |
| Dan Hipschman | 2007-10-03 | [widl: Add a declonly argument to write\_type\_left.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32a2477ef574546a2ce1fbfdf2e327d7a5298a16) |
| Dan Hipschman | 2007-10-03 | [widl: Write types in the format string comments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=304852f97e8da64954e33ceb6ab5e014fa26049f) |
| Roy Shea | 2007-10-02 | [net.exe: Added missing service name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8c43acc2b5dba5cf1b30777daad522f34ffbf31) |
| Dmitry Timoshkov | 2007-10-02 | [user32: Add a message test for ownerdrawn listbox, make it pass under Wine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a218e97affb928d5d7d4eba8d89670d4603769f) |
| Alexandre Julliard | 2007-09-27 | [winex11.drv: Always drag the full window for top-level windows to avoid having to ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e36ed76139a37aa1439048ee642acfdbfd25c28c) |
| Dan Hipschman | 2007-09-27 | [widl: Fix array alignment bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cbd75d3ace9a4d06a16837bea5b046ba1122aeb0) |
| Jacek Caban | 2007-09-26 | [mshtml: Added IHTMLDocument5 interface stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ba65105d54224cd9551819189a6946e7ccd014f) |
| Dan Hipschman | 2007-09-26 | [widl: Fix string codes in pointer descriptions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=723c8bacfaba0c945f889eaf8861e94385878f40) |
| Miko&#x0142;aj Zalewski | 2007-09-26 | [shell32: shlview: Change some more ANSI calls to Unicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4db3b1bba868924665258d80c138d4c9655b90a3) |
| Dan Hipschman | 2007-09-26 | [widl: Fix top-level conformant arrays with pointer attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=347f2a2da2b98d8e365f944e439c9b8ee54ee30d) |
| Miko&#x0142;aj Zalewski | 2007-09-26 | [shell32: Make the shell view control Unicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=212c36048a381af11b424a6fe901d69de92a760b) |
| Dan Hipschman | 2007-09-25 | [widl: Clean up write\_conf\_or\_var\_desc with string\_of\_type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb3275ce97c44346879ae8a2759d64f92af4e47a) |
| Miko&#x0142;aj Zalewski | 2007-09-23 | [advapi32: Add some more rights constants for ConvertStringSecurityDescriptorToSecurit ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b4aa62fd2ae961a2c4017d766b728b834b705cc) |
| Juan Lang | 2007-09-21 | [setupapi: Create symbolic link value when interface is created.](http://source.winehq.org/git/wine.git?a=commitdiff;h=df3cb0630df098cab0aa7f422c40ff813e91bd93) |
| Juan Lang | 2007-09-21 | [setupapi: Add test showing value of path.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d34ec8b8a121ed05e7859827f55a385727349e26) |
| Juan Lang | 2007-09-21 | [setupapi: Add stubs for SetupDiCreateDeviceInterfaceA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1878ab8fd9aab52d0d1763cc99e61b5ec4134fb) |
| Juan Lang | 2007-09-21 | [setupapi: Implement SetupDiEnumDeviceInterfaces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be863b07ff157556beed1d3a66a60942d86a9cba) |
| Juan Lang | 2007-09-21 | [setupapi: Implement SetupDiCreateDeviceInterfaceA on top of SetupDiCreateInterfaceW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa2b23cab5aeabc893d9d635848f7357064614e0) |
| Juan Lang | 2007-09-21 | [setupapi: Respect samDesired in SetupDiOpenClassRegKeyExW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a9d74cf994d0a3853373799e9a1456a0b7a47bb8) |
| Juan Lang | 2007-09-21 | [setupapi: Implement SetupDiGetDeviceInterfaceDetailA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a63c9356a4fcaeea42eb31752c6ac0323b75daf2) |
| Juan Lang | 2007-09-21 | [setupapi: Set last error on failure in SetupDiOpenClassRegKeyExW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b1e1b2aadcdebf09ef306677844701d6177cf82) |
| Juan Lang | 2007-09-21 | [setupapi: Add tests for SetupDiCreateDeviceInterface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8069619b907564345ea8fa07d63d92856cff09bc) |
| Juan Lang | 2007-09-21 | [setupapi: Set last error on invalid input.](http://source.winehq.org/git/wine.git?a=commitdiff;h=707fca6cbce5d9e387112738339e54a4f2697712) |
| Juan Lang | 2007-09-21 | [setupapi: Add tests for SetupDiGetDeviceInterfaceDetail.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6bd4ed73cb04c67614baad9e74c0cfb8db82bd12) |
| Juan Lang | 2007-09-21 | [setupapi: Implement SetupDiCreateDeviceInterfaceW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69b0b424550c35d5f74508975f47907ed56b1686) |
| Juan Lang | 2007-09-21 | [setupapi: Add error checking to SetupDiCreateDeviceInterfaceW stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=66820122091fa678804fabd75daec4deb10316ef) |
| Juan Lang | 2007-09-21 | [setupapi: When enumerating an interface, add the interface to its device.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50a4039037b0b3c7a01da3462c5791e9e0a129d1) |
| Juan Lang | 2007-09-21 | [setupapi: Remove a redundant parameter check.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15eba01660040d7bd4effd5f6eab5cf285fac3c9) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiGetDeviceInstanceIdW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f94f6367f2f4ada5bfb1fe973c6836b2b2e71dbc) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiGetClassDevsW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f841667cac1558d2131543c5dc9baba1c6418b01) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiRegisterDeviceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4b9bc2454b6c996ea601a2ae3d3ce80b8225273) |
| Juan Lang | 2007-09-20 | [setupapi: Add tests for SetupDiGetDeviceInstanceId.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e481b1eaee50b86071bcafffbebb746418e86fe4) |
| Juan Lang | 2007-09-20 | [setupapi: Make a helper to convert a GUID to a string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e1449796973d67a204e72f6b43124c9f5f2609f5) |
| Dan Hipschman | 2007-09-20 | [widl: Respect pointer attributes better.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dbfabf68a2c36a554c44589b55ef0dbab24ef4b6) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiGetDeviceInstanceIdA on top of SetupDiGetDeviceInstanceIdW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1ccd65792cc003bcac08d5ceeaac17b80447919) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiGetDeviceRegistryPropertyA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc924f5b3a02316f71b70653da4c953ba00f557e) |
| Juan Lang | 2007-09-20 | [setupapi: Add a placeholder for devices.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a7ad54ef9243a618a55dbaf8815363aa62da3e6c) |
| Juan Lang | 2007-09-20 | [setupapi: Add tests for SetupDiRegisterDeviceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a57a17d3fc012dd97b9931de68bc0a118a0bb868) |
| Juan Lang | 2007-09-20 | [setupapi: Save device description to registry when creating a device.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8985a62a340a7f1fdd44c91c878d0c94a0af5474) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiCreateDeviceInfoW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83f05e79bb77785a101c458100dc227738abda6e) |
| Juan Lang | 2007-09-20 | [setupapi: Devices created by SetupDiCreateDeviceInfo are &quot;phantoms&quot;, and are deleted ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=80be1fe74007ff207480036ee8596809eb3dae5d) |
| Juan Lang | 2007-09-20 | [setupapi: Add stubs for SetupDiGetDeviceInstanceIdA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c0a3117535d1a4b9a724ab2494c3de434fea248) |
| Dan Hipschman | 2007-09-20 | [widl: Handle top-level conformance for complex arrays.](http://source.winehq.org/git/wine.git?a=commitdiff;h=767a1f26f6249b485a6aa09467ac1d45174214c8) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiGetClassDescriptionExA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6b50538f123d0b62e773f749dd32a18bd8e3157f) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiEnumDeviceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=634cba84d2fc548594276a26d672e4117a527956) |
| Juan Lang | 2007-09-20 | [setupapi: Implement SetupDiSetDeviceRegistryPropertyA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60fefd72e8330e2942235309e3cd3ea2604c7a4c) |
| Juan Lang | 2007-09-20 | [setupapi: Add stub for SetupDiRegisterDeviceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a2a99474e23c40a0fb302382cec744ecaef7ccc) |
| Juan Lang | 2007-09-20 | [setupapi: Add tests for SetupDiCreateDeviceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=362e8e1f62657e4de041f2f8e0c9c9e34703dcab) |
| Dan Hipschman | 2007-09-20 | [widl: Set the pointer description offset to zero if there are no pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33da66d6c8c829ded8059dd3aeb1549081d76c23) |
| Juan Lang | 2007-09-20 | [setupapi: Add error checking to SetupDiCreateDeviceInfoW stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1bbfd72afbda1e1b953ac6fef7a396ba5b518209) |
| Juan Lang | 2007-09-20 | [setupapi: Save class GUID to registry when creating a device.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00ef2e3269a51e5817121ee47b3e18d9e58e77d5) |
| Alexandre Julliard | 2007-09-19 | [winex11.drv: If a window is not resizable through the window manager fall back to ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d21e6b37517d77cfc051005ebb3efaf479f9bc3) |
| Juan Lang | 2007-09-18 | [crypt32: Simplify AsnDecodeSequenceItems a tiny bit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f534a67bfc59d3b8b74d69cfcc4e60411f293104) |
| Juan Lang | 2007-09-18 | [crypt32: Temporarily change prototype of AsnDecodeIntInternal to the CryptDecodeObjec ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2bff633acb55d3ee8d12ee207aafd510058034b) |
| Juan Lang | 2007-09-18 | [crypt32: ret is already true, don't retest it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee28204fcf37c39786bcb865da55eed1e93a6160) |
| Juan Lang | 2007-09-18 | [crypt32: Use internal form for all internal decoding functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e03864a205ec084fb313ccdea855f4ca4179bd65) |
| Juan Lang | 2007-09-18 | [setupapi: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d62285d006389c2a17e1d1b33f2ffcb6bd0f3ba0) |
| Juan Lang | 2007-09-18 | [crypt32: Get rid of encoding type argument to AsnDecodeSequence, it isn't used.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce47433d94d2dffc6f0bb45f053375d2942400f2) |
| Juan Lang | 2007-09-18 | [crypt32: Simplify DecodePathLenConstraint.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be91ad360437363bf91aae977a95d8244df8dee9) |
| Dan Hipschman | 2007-09-18 | [widl: Fix alignment comments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b16de39417aad0393257370f52d05e07e362a9e2) |
| Juan Lang | 2007-09-18 | [setupapi: Correct type to match PSDK.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae6f5616cb3dabaf47e3b48602db976d5ba6b0e7) |
| Juan Lang | 2007-09-18 | [crypt32: Implement DecodeAltName with DecodeAltNameInternal.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad94982284f4d7db57c4c1c4f66b80be01f9b3ce) |
| Juan Lang | 2007-09-18 | [crypt32: Use simpler form for internal time decoding functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a538e95c1d77694ce4a4f2ddc40de11c534d8131) |
| Juan Lang | 2007-09-18 | [setupapi: Add missing prototypes and definitions, and change function prototypes ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=9fc7973727e9140f92188d5624e8e44600cb9065) |
| Juan Lang | 2007-09-18 | [crypt32: Move a comment that belonged elsewhere.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d0dccf164c508c3d98ec03bb78aab5752763bc3) |
| Juan Lang | 2007-09-18 | [crypt32: Explicitly count bytes to copy in DecodeCopyBytes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c4c856fde5370c515714f0a81a7dc50ac647838) |
| Juan Lang | 2007-09-18 | [crypt32: Fix alignment for 64-bit systems.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91f2a4d687dcbab4539aa4f9db5d8982cfd95ade) |
| Dan Hipschman | 2007-09-18 | [widl: Implement pointer descriptions for complex structures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8df79f0c999c4736326f381b59de8b31cf894beb) |
| Juan Lang | 2007-09-18 | [crypt32: Introduce a space checking helper for functions that don't allocate memory ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c5bd5f5ca6c2543d7a20a2761e0f5b78bff4f1f) |
| Juan Lang | 2007-09-18 | [crypt32: Use AsnDecodeIntInternal where an internal function is called for.](http://source.winehq.org/git/wine.git?a=commitdiff;h=89a541a493ca5352d2cae6c3ef88e3f627d2f176) |
| Juan Lang | 2007-09-18 | [crypt32: Test and correct decoding indefinite-length-encoded PKCS content.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e475b4a774edf29d7c3ae5def5f0d0f5d159368) |
| Juan Lang | 2007-09-18 | [crypt32: Implement streamed encoding of an indefinite-length data message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71b5ba03362dfaf3dc3ebda43a51e7f223ae2f6b) |
| Dan Hipschman | 2007-09-18 | [widl: Handle all buffer sizes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6eb07cb100086ce52fe83d3134899a197b7b71e6) |
| Juan Lang | 2007-09-18 | [crypt32: Separate DecodeInt into an internal and external version.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5fbca384e4eb15af4f96fe3e27f6001eee4c5597) |
| Juan Lang | 2007-09-18 | [crypt32: Allow items in an array to be indefinite-length encoded.](http://source.winehq.org/git/wine.git?a=commitdiff;h=52be131a2904989ffad66acf0eae9269fed83c45) |
| Juan Lang | 2007-09-18 | [crypt32: Allow a sequence to have an indefinite-length encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fd90ddad335c3eb6f9ae74bebce95d65d97e960) |
| Juan Lang | 2007-09-18 | [crypt32: Use correct encoded length when decoding a sequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43e6b48b33026bfb67c3b7a5863a7e525ff7450c) |
| Juan Lang | 2007-09-18 | [crypt32: Allow indefinite-length encoding of sequence items.](http://source.winehq.org/git/wine.git?a=commitdiff;h=34aaabca830018d6a5212e0a91f3a25032601fc3) |
| Juan Lang | 2007-09-18 | [crypt32: Set \*pcbDecoded in every function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2e8ae598e11ee1c87e51b02ce7bea63f52b94646) |
| Juan Lang | 2007-09-18 | [setupapi: Fix return type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2e2fe9b9f786479e5285504b6a98d6cdf96c00ed) |
| Juan Lang | 2007-09-18 | [crypt32: Don't use exception handler when decoding time zone, caller already does.](http://source.winehq.org/git/wine.git?a=commitdiff;h=21246938c4ce4442e9e5ed59efd4fa721b42166a) |
| Juan Lang | 2007-09-18 | [crypt32: Use internal decode int function a couple more places.](http://source.winehq.org/git/wine.git?a=commitdiff;h=205c733b1309f0291bcaa2b0a0027ac8257128af) |
| Juan Lang | 2007-09-18 | [crypt32: Get rid of encoding type from AsnDecodeSequenceItems, it's never checked.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19fd9872a669147e14cff3adc4dbdcc7e5f74fa9) |
| Juan Lang | 2007-09-18 | [crypt32: Pass length rather than entire message to CRYPT\_EncodeContentLength.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19956d6e97a57962cde6a063cbc2ca571b58589a) |
| Dan Hipschman | 2007-09-18 | [widl: Implement complex arrays.](http://source.winehq.org/git/wine.git?a=commitdiff;h=132f06cd48c7ebd176649a5e00795e7a7fc67adb) |
| Juan Lang | 2007-09-18 | [crypt32: Use decode function's returned decoded length to advance pointer when decodi ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0bd29b124310e9797f66ddd162f574ecad237e99) |
| Juan Lang | 2007-09-17 | [crypt32: Return bytes decoded when decoding a sequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd982c85976819bec370e13d3a99ac78a17d99aa) |
| Juan Lang | 2007-09-17 | [crypt32: Add a decoded parameter to AsnDecodeSequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f3490f3ed8bcbf80aba08916a349ba34541d1eb6) |
| Juan Lang | 2007-09-17 | [crypt32: Correct GET\_LEN\_BYTES for the indefinite-length form.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e747f706b1d7f87d12c48ed49d2f465e1b2f1537) |
| Juan Lang | 2007-09-17 | [crypt32: Return bytes decoded from AsnDecodeArray.](http://source.winehq.org/git/wine.git?a=commitdiff;h=deb07ccb1c5258e2097b591263cd6993a893bba3) |
| Juan Lang | 2007-09-17 | [crypt32: Return bytes decoded when copying DER-encoded bytes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7e8eed94464649c270a592b209b13f2cdf702eb) |
| Juan Lang | 2007-09-17 | [crypt32: Fix alignment on 64-bit systems.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc2059b67c5734e9193c489eadce9916eda64f04) |
| Juan Lang | 2007-09-17 | [msi: Don't crash if record has no fields.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2d66da665984e6dbfa462baa935b211c1c8b146) |
| Juan Lang | 2007-09-17 | [wininet: Create a TCP connection if FLAG\_ICC\_FORCE\_CONNECTION is specified.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba45902dafc8fabd93ce49e2d8bcf4cc9d946e33) |
| Juan Lang | 2007-09-17 | [crypt32: Pass bytes decoded pointer to AsnDecodeArray.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2f02f3bf778412b747d70ed91ce5fe3cb7d1390) |
| Juan Lang | 2007-09-17 | [msi: Initialize nested.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3331c6f2278489826be35a46620cead4f9c3c07) |
| Juan Lang | 2007-09-17 | [crypt32: Introduce a helper function to get encoded length that allows indefinite ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7ecf5becbd9ce7f62a80cc4294db1f44a62a17c1) |
| Juan Lang | 2007-09-17 | [crypt32: Use a simpler prototype for array decoding functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=731d37b049027afd44241d05cd9e4487fe1086d0) |
| Juan Lang | 2007-09-17 | [msi: Make sure nested is initialized.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71a78c4478aa277333e71c36a88a1c0297093c78) |
| Juan Lang | 2007-09-17 | [crypt32: Update comments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=716a7405e47c1f4019a6286d723e5611e00d5a9b) |
| Juan Lang | 2007-09-17 | [crypt32: Support indefinite-length encoded arrays.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d168bd4c0fe9725114a652175ffcab01a25fb91) |
| Juan Lang | 2007-09-17 | [crypt32: Remove an unneeded WINAPI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54a51afcd77891353400499fc3bd69c81cf5cdf7) |
| Juan Lang | 2007-09-17 | [crypt32: Return bytes decoded when decoding an alt name entry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f4bcb4a3dd9dba6c4fa92ac880d62efb7a31cfa) |
| Juan Lang | 2007-09-17 | [crypt32: Make a decode OID function that returns the number of bytes decoded.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1dd1c6c2c89bd9afae39a2405ce3663025dd0e30) |
| Juan Lang | 2007-09-17 | [crypt32: Add a test of an indefinite-length sequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15b19f1d1637dce7f56c3e1a71e11811cd0013de) |
| Juan Lang | 2007-09-17 | [crypt32: Set bytes decoded in all success paths.](http://source.winehq.org/git/wine.git?a=commitdiff;h=159a369318ce4e0a1e9223bd92c6cdcf920bd40f) |
| Juan Lang | 2007-09-17 | [crypt32: Correct an optimization.](http://source.winehq.org/git/wine.git?a=commitdiff;h=09447fb605d9ea302bb6cdd1bc7fef7d9791a58a) |
| Dan Hipschman | 2007-09-14 | [widl: Add padding to the end of complex structures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e84eb9a475a10410b6ad56c029ef1023fa44d9c) |
| Dmitry Timoshkov | 2007-09-12 | [shell32: Remove class cache introduced in commit f686cfab2feb9010efe82a932dc9f5904566 ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e3cfd6ef32d1e298879b1b1b15f0a039dd04bc6b) |
| Dan Hipschman | 2007-09-12 | [widl: Fix an unused parameter warning on write\_conf\_or\_var\_desc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce4055c573151de710b875443dc1b8435ab9a772) |
| Juan Lang | 2007-09-12 | [wintrust: Implement SoftpubCleanup.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b13d16a0da4f02c577bc8b4ee02e5124e749ad19) |
| Juan Lang | 2007-09-12 | [wintrust: Don't prefer native version.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae8e8a0a57954f4091c147e91d9fc78d206bbc79) |
| Dan Hipschman | 2007-09-12 | [widl: Use the correct functions for interface pointers in stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7deb62505cc80c8412e319238351fc0d59810d50) |
| Juan Lang | 2007-09-12 | [wintrust: Implement WinVerifyTrust.](http://source.winehq.org/git/wine.git?a=commitdiff;h=40f33d656819085d585943a2f38b9ad2a50f9132) |
| Juan Lang | 2007-09-12 | [wintrust: Save signer cert so chain can be created.](http://source.winehq.org/git/wine.git?a=commitdiff;h=277ef05efb3431b4f1b34266d9d0e9283e1eb693) |
| Dan Hipschman | 2007-09-12 | [widl: Add calls to NdrFooFree for more types in server stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=177346f1b6825a4f7425369612004402d6a0ef12) |
| Juan Lang | 2007-09-12 | [wintrust: Partially implement SoftpubAuthenticode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0463f99b73ea92a6532ae38e5bf00d633049228c) |
| Juan Lang | 2007-09-11 | [rsaenh: Validate pad byte when decrypting a block cipher.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0d2766fdc945fc967e5efbedbab9e022baabf4a) |
| Juan Lang | 2007-09-11 | [crypt32: Make chain tests more strict.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0add110077451403b45cbc8ff0e18b2e5d91739) |
| Juan Lang | 2007-09-11 | [crypt32: Set subject's info status from method used to find issuer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5833ac9f42b0968c44492c55b29903be085eb5d) |
| Juan Lang | 2007-09-11 | [crypt32: Only decode authority key ID in subject cert once when looking for issuer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c8254886f087a22e3648a87f6494184941b74ae) |
| Juan Lang | 2007-09-11 | [crypt32: Pass subject's info status when adding an issuer to a chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54428bfb99b8396d7027a20dd56f276169a73df3) |
| Juan Lang | 2007-09-11 | [crypt32: (Re)introduce helper function to get issuer certificate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05492ae9073eac48bbcf63cfe2edac7e80275aed) |
| Juan Lang | 2007-09-10 | [crypt32: Add initial tests for CertVerifyCertificateChainPolicy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f23ec305344dca2ea62a432785358a58af7baa87) |
| Juan Lang | 2007-09-10 | [crypt32: Support CRYPT\_DECODE\_TO\_BE\_SIGNED\_FLAG.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7115ce33c7ffb393cd6853010dd8e63ba2db88a) |
| Juan Lang | 2007-09-10 | [crypt32: Implement CertVerifyCertificateChainPolicy for the base policy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b56f0c5b687043bd8c8d09d1773bd606800b35a0) |
| Dan Hipschman | 2007-09-10 | [widl: Output UUID files compatible with older Visual C++ and MinGW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d2c6e78f2ae1e263dabbcc03e7cf267f2d3685a) |
| Juan Lang | 2007-09-10 | [crypt32: Add a root store implementation that reads trusted certificates from well ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=9663f9427b10e1d82bc98b03b07d688d09f64dd2) |
| Juan Lang | 2007-09-10 | [crypt32: Add a stub for CertVerifyCertificateChainPolicy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91c76955e7db93606f3e8a92ba844fe618c11745) |
| Juan Lang | 2007-09-10 | [crypt32: Add policy flags definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8bc15e7b4a156316775744edbb79f7ea17e5381e) |
| Juan Lang | 2007-09-10 | [crypt32: Implement CertVerifyCertificateChainPolicy for the authenticode policy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5f06293eb10f21ef852a267235023ed8f5a6cea8) |
| Juan Lang | 2007-09-10 | [rsaenh: Call setup\_key whenever the IV is reset.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5666efb1374bb0a1e7f9d92614f9c6956ac9eca3) |
| Juan Lang | 2007-09-10 | [rsaenh: Support setting the effective key length of RC2 keys.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41d057837cd7c22ba2db55690add4761865e0e24) |
| Juan Lang | 2007-09-10 | [crypt32: Add a function to create a certificate chain engine potentially before the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=391f826d49604f2bc70bf2574e2273307f139d48) |
| Juan Lang | 2007-09-10 | [rsaenh: Reorder padding code to avoid unnecessary comparison.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16c40d91124547499a289df8efffba2e9d1effb5) |
| Juan Lang | 2007-09-10 | [crypt32: Implement CertVerifyCertificateChainPolicy for the basic constraints policy.](http://source.winehq.org/git/wine.git?a=commitdiff;h=039beff4415cc6b92aa2ed19619f0d66bcfaf1d8) |
| Juan Lang | 2007-09-06 | [crypt32: Open world store when creating chain, not when building a simple chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e9ee8c8717833dcd4c580451477f48df4d6efc8f) |
| Juan Lang | 2007-09-06 | [crypt32: Don't abort chain creation if the root signature isn't valid.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfd2d3d9bc3785c2a0051dc94bca4adb7a60a12c) |
| Juan Lang | 2007-09-06 | [crypt32: Remove a misplaced todo\_wine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d82f3f37a2160fbacc852152eefe6a464bdfac87) |
| Juan Lang | 2007-09-06 | [crypt32: Separate allocating a simple chain and checking it from building it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4e07a5bfc4cb298bbcc05d7e7d122c6be3da80f) |
| Juan Lang | 2007-09-06 | [crypt32: Store world store in chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a82b36ac9811dcec46f0db1967d4fec357522ff2) |
| Juan Lang | 2007-09-06 | [crypt32: Defer checking signatures until chain is complete.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a040dd22e75f8ca86961a0a0afbc0caa97c9f109) |
| Lei Zhang | 2007-09-06 | [riched20: Do not pass NULL lParam to ME\_ToUnicode for EM\_REPLACESEL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9210defdf77e6db5830fdb1206fb077df60ce00f) |
| Juan Lang | 2007-09-06 | [crypt32: Don't add end cert's store to world.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8698a598fc8aa2094caa1800ec13e8de19ac087e) |
| Juan Lang | 2007-09-06 | [crypt32: Not finding an issuer shouldn't cause chain creation to fail.](http://source.winehq.org/git/wine.git?a=commitdiff;h=818634d69a4c3979b43d467818a319208053d709) |
| Juan Lang | 2007-09-06 | [crypt32: Add more tests for getting issuer cert from store.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6aa03fc4c314671234975aecdb1afa81233d7427) |
| Juan Lang | 2007-09-06 | [crypt32: Set \*ppChainContext even on error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69834b16accf0fcb7335ee7c807486b86d2997db) |
| Juan Lang | 2007-09-06 | [crypt32: Consider alternate issuers when building chains.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e674f3580d629a3a5e0ef82df4db4fb16efd491) |
| Juan Lang | 2007-09-06 | [crypt32: Add special case for certificates with no signature algorithm.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b029479379da1a53d76b751de212ed02501f25d) |
| Juan Lang | 2007-09-06 | [crypt32: Don't ask CertGetIssuerCertificateFromStore to verify revocation status, ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=56d4a3c3924917253b401c6c2920a932072f0bee) |
| Juan Lang | 2007-09-06 | [crypt32: Test whether chain creation should fail when a root signature is invalid.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31618f91dd3db6c05627ea85768d4858ac67b1c5) |
| Juan Lang | 2007-09-06 | [crypt32: Flags weren't set, so don't bother passing them.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1fc8c6078899ea973930434a4e45e49779410926) |
| Juan Lang | 2007-09-06 | [crypt32: Make a helper function to create initial candidate chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a059879bf0d0df531646238c676daedfde329b9) |
| Juan Lang | 2007-09-06 | [crypt32: Test that the end cert in a chain's store isn't implicitly searched for ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=192ed7353d15dbd45047945ce8813f9b6cb3b77a) |
| Dan Hipschman | 2007-09-04 | [widl: Allow size\_is on strings.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba54c455fbb312817e0896dd422f7fe721a5099e) |
| Dan Hipschman | 2007-09-04 | [widl: Implement NDR for struct field alignment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62fb623e14498716730eea347a999256b9707803) |
| Dan Hipschman | 2007-09-04 | [widl: Fix top-level and callback conformances.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d036da6d3c657bc49119079171a1eef8204f8a8) |
| Juan Lang | 2007-08-31 | [crypt32: Time validity nesting doesn't appear to be checked, so don't check it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d06a24517f63caab722a180bedf920d1602cff29) |
| Juan Lang | 2007-08-31 | [crypt32: The preferred issuer flag appears to be a bug in XP, so don't set it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf2047fd726d643638d8191cc9836cbd24c3e163) |
| Juan Lang | 2007-08-31 | [crypt32: Don't fail chain creation if signature doesn't match.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c39696eb14c9a61ecf5fe14a394f0b89dd96b104) |
| Juan Lang | 2007-08-31 | [crypt32: Halt chain creation when a cycle is detected.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8b787a81039c4a62c04540d2529593cf3f5fa87) |
| Juan Lang | 2007-08-31 | [crypt32: Check chain root's trusted status regardless of whether its signature is ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4e88cb64402e602ab1a61f859bc8eaafdc5c139) |
| Juan Lang | 2007-08-31 | [crypt32: Properly reference count certificate contexts referenced by a chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8cd7abf1be287af002e742cf2a06a0d83364baa4) |
| Juan Lang | 2007-08-31 | [crypt32: Check path length constraint on a chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c9b788fb89e4b4b41b357981e169397b8216266) |
| Juan Lang | 2007-08-31 | [crypt32: Greatly expand certificate chain tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a8a7362cc1dae3237b7e92ea4db2a8b44df79d4) |
| Juan Lang | 2007-08-31 | [crypt32: Implement CertDuplicateCertificateChain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51a9d208eebf1f0e61f5035e30c0bf50f843bd35) |
| Juan Lang | 2007-08-31 | [crypt32: Check time of each element in chain against requested time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51948b0c980e6f7a9e2725958c16f8c712bfcc69) |
| Juan Lang | 2007-08-31 | [crypt32: Add a default cycle detection modulus.](http://source.winehq.org/git/wine.git?a=commitdiff;h=45eef63a35f27a522e4c3e24f2511593bffb987c) |
| Juan Lang | 2007-08-31 | [crypt32: Remove unneeded WINAPI from internal function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ef4c7e1ccbbd331c5283e8ecd92cc51edc6333d) |
| Juan Lang | 2007-08-31 | [crypt32: Check whether each signing certificate can be a CA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ce46d5e4a38b9be67b442747ab6952a0bf44a88) |
| Juan Lang | 2007-08-31 | [crypt32: Don't fail chain creation if root isn't self-signed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1540f24e9247a7418449b43aa45068afca1f76ed) |
| Juan Lang | 2007-08-31 | [crypt32: Set error status on issued certificate, not on issuer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14b0df1fef5258ab6bb84acde166389cdc7947e5) |
| Juan Lang | 2007-08-31 | [crypt32: Free lower quality chain contexts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0dc82780cab6583935abcc811ef912cd215b1767) |
| Juan Lang | 2007-08-31 | [crypt32: Correct combining trust status of a chain's elements into the chain's trust ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=03d76d97ecc427d534069c5e0194ca0eadacfcca) |
| Juan Lang | 2007-08-29 | [winerror.h: Add more error definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a47f47fe294a2ad6aede0bd79c1d468d150b2b53) |
| Dan Hipschman | 2007-08-29 | [widl: Handle the size\_is attribute on pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d73123dbc8c262025783a15d1bb4eca271f8b81) |
| Juan Lang | 2007-08-28 | [wintrust: Use a helper function to get a signer's cert info from a message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fb07a3aa02cfb3329bce4a08b7d4e8f45e93bbe0) |
| Juan Lang | 2007-08-28 | [crypt32: Set trust status on root element in chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eda48d8868065d2d7debafa79ba25fd8e1d8bc59) |
| Dan Hipschman | 2007-08-28 | [widl: Handle LPSTR in typelibs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d82b384859c9d87827a35151e14f8ca2365e8a57) |
| Juan Lang | 2007-08-28 | [wintrust: Implement pfnCertificateTrust.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b157166345693d9b4b6eceafd6edaa79c3512381) |
| Juan Lang | 2007-08-28 | [wintrust: Use pfnAddStore2Chain internally.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4d85d80a37967a57df85ee9b9d8be8a6fbb4e3e) |
| Juan Lang | 2007-08-28 | [wintrust: Test and implement pfnAddSgnr2Chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c34271aaa54165e8b9ecb1395b0836e3de9388a) |
| Juan Lang | 2007-08-28 | [wintrust: Save signers of a message in SoftpubLoadSignature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d7bffa5c7117dbdd3849b3141c69445cc8cf08c) |
| Juan Lang | 2007-08-28 | [wintrust: Test and implement pfnAddCert2Chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f2fae1d991b08d2150709c3b16ef8fec50b7e2a) |
| Juan Lang | 2007-08-28 | [wintrust: Add missing definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3db50276ab66c87ea9e8ab8548dcc5f06d6afe3c) |
| Juan Lang | 2007-08-28 | [wintrust: Test and implement pfnAddStore2Chain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=150ddd6bd48540dbf5bd92f3bd9b94fc7f605564) |
| Juan Lang | 2007-08-27 | [wintrust: Implement SoftpubLoadSignature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=92de4384690fd86f2b7951d5c3e5a9850ac85fca) |
| Juan Lang | 2007-08-27 | [wintrust: Move mem alloc functions to wintrust\_main.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f8b296fb18d904ea5f064dd4209df7bdfcebed9) |
| Juan Lang | 2007-08-27 | [wintrust: Test and implement SoftpubLoadMessage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a3fb3b566875b4ba52430e460e14318db3a469f) |
| Juan Lang | 2007-08-27 | [wintrust: Use common memory functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=492518d03729179ccc05d9315b4fa3bb4f314e02) |
| Juan Lang | 2007-08-27 | [imagehlp: Move WIN\_CERTIFICATE types to wintrust.h, and rename a type, to match PSDK.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01b083c5758b25a1ba7d495033f9abac2633d273) |
| Dan Kegel | 2007-08-25 | [shdocvw: iexplore needs to handle the -nohome option.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e0ece41a580f511e6e416cb2485eedeac9736c1) |
| Juan Lang | 2007-08-24 | [crypt32: Partially implement CMSG\_CTRL\_VERIFY\_SIGNATURE\_EX.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff26d428e3e59ed4e8e1a04411ed692c47254cb4) |
| Juan Lang | 2007-08-24 | [wintrust: Test and correct alloc and free functions in WintrustLoadFunctionPointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e8cc4db1c75694ea3f887cea46ff0e53a1a2eb13) |
| Juan Lang | 2007-08-24 | [wintrust: Add trust step error definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb963cc92060115b458bf229bcad65028e05b6eb) |
| Juan Lang | 2007-08-24 | [wintrust: Test and implement SoftpubInitialize.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7850caa714784d0e168efcacc45d359498881e4a) |
| Juan Lang | 2007-08-24 | [wintrust: Make crypt provider functions calling convention explicit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=67a0ff46eb40ba0376425bc47a564c2f237065bc) |
| Lei Zhang | 2007-08-23 | [gphoto2: Import photos in the right order.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ffbca82668fcf16d1ebb82669b244f2a6c64a0f7) |
| Lei Zhang | 2007-08-23 | [gphoto2.ds: Add preview button and ability to disable import GUI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e2605fb0ed517cc2ea03a18cb3f94bda5629321f) |
| Nigel Liang | 2007-08-23 | [winecfg: Suport color schemes from .theme format themes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=998baf9f0fe4723b0171f03626687ef1e541a344) |
| Lei Zhang | 2007-08-23 | [gphoto2: Add missing brackets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4945a255e40d90b755cde1f35caea00f9d30009a) |
| Juan Lang | 2007-08-22 | [crypt32: Implement CryptVerifyMessageSignature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5b4806159deb89a5d340145b16ec5fce935b537) |
| Juan Lang | 2007-08-22 | [advapi32: Add more tests for CryptVerifySignatureW, and correct its parameter checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5bbed2b95abb5b8983df487c62039c683fe98cb) |
| Juan Lang | 2007-08-22 | [crypt32: Test and correct verifying the signature of a valid signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a9e1d66480c85c98c72c4ebd9710bb297ae3091) |
| Juan Lang | 2007-08-21 | [crypt32: Make constructing handles a member of signed msg data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1f8e87b332489fb710c90d9473d668223f7e424) |
| Juan Lang | 2007-08-21 | [crypt32: Update a hash message's hash handles when decoding it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed6fbb2712206e671500debbd9946c3ef91ddf34) |
| Juan Lang | 2007-08-21 | [crypt32: Add a couple tests that show you can't get the hash from an encoded hash ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7ce5ae2bcca233dede16ccaa675036dcfd9b9e1) |
| Juan Lang | 2007-08-21 | [crypt32: Test and implement CryptGetMessageSignerCount.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e52c80e53b67d00750537dc87238f0e6d51ed281) |
| Juan Lang | 2007-08-21 | [crypt32: Add helper function to update signed message data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=de88fedcce46fa51e3b84e8819882c1faa75c386) |
| Juan Lang | 2007-08-21 | [crypt32: Only free allocated handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4c318f2952d0f0fee446ee9ca3273c9acf1e6ed) |
| Juan Lang | 2007-08-21 | [crypt32: Test and implement getting the computed hash from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3431271faf13454f278ace4950d41caab68e428) |
| Juan Lang | 2007-08-21 | [crypt32: Move signed message data functions together.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d2dc7d78a9e6f6e7c925cc254961849132634d12) |
| Juan Lang | 2007-08-21 | [crypt32: Add tests for CryptMsgControl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc8948fefab090237fb83eabbe324d9f74b2a734) |
| Juan Lang | 2007-08-21 | [crypt32: Add a helper function to construct a signer handles structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4dd74d84c8bf2f52532ae76eb7e32a61d682dcc) |
| Juan Lang | 2007-08-21 | [crypt32: Make updating a hash a member of signed message data, not signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bfde05d8b69f12b00f5cc286110f2388fa33ed1f) |
| Juan Lang | 2007-08-21 | [crypt32: Separate construction of signer handles from signer info.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bfbc159d1e0bb55de630748c65c98a22a3fc8a61) |
| Juan Lang | 2007-08-21 | [crypt32: Implement CryptGetMessageCertificates.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b9038be1ff6ca6f35db2756443cb232f7a144bba) |
| Juan Lang | 2007-08-21 | [crypt32: Implement verifying a decoded signed message's signature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7e420429db8e3a2eab503f49ce0b04a4ac7f551) |
| Juan Lang | 2007-08-21 | [crypt32: Trace encoding and decoding public keys on crypt channel.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6032a41b3c9768b3d6c47e50ea4c71c6b989fa2) |
| Juan Lang | 2007-08-21 | [crypt32: Test an encoded signed message with a cert with a public key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c4330e732e7fec10b4b5310879a21b8f4b5666e) |
| Lei Zhang | 2007-08-21 | [wine.inf: Add twain\_32.dll to the list of fake dlls.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8942b7888be73847b77e1ad79f99afa49a88c5a2) |
| Juan Lang | 2007-08-21 | [crypt32: Make a signed message data type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7748905743a497ac5215f9289b555061406675d2) |
| Juan Lang | 2007-08-21 | [crypt32: Explicitly terminate loop when a matching signer cert is found.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6acd76164617ecb3391a4449b88080129d756339) |
| Juan Lang | 2007-08-21 | [crypt32: Use signed message data type for decoded signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e9299d980fc240a2781bcfc4de0c9ac6282aa3a) |
| Juan Lang | 2007-08-21 | [crypt32: Test encoding a signed message with a valid public key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fb26709cd631bc24ca27acdc47f8f7b770a56a4) |
| Juan Lang | 2007-08-21 | [crypt32: Implement verifying the hash of a decoded hash message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3e88838b606a93c67e92ee1a50e5b1d53a8df730) |
| Juan Lang | 2007-08-21 | [crypt32: Add a default message control function pointer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31c414f4b483c424dbf7244ad3dca08651b2a667) |
| Juan Lang | 2007-08-21 | [crypt32: Don't keep an unneeded copy of the crypto provider for each signer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f9d9be7625fca4917916fdd334a254dd78ffb85) |
| Juan Lang | 2007-08-21 | [crypt32: Add a mostly stub control function for decode messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=163e8d6256224fa4e6bc65a3f7ddc434b97bfdf8) |
| Juan Lang | 2007-08-21 | [crypt32: Make more functions members of signed message data, rather than message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1522282673e19f6cb31b775bafd8cb564e05d138) |
| Juan Lang | 2007-08-21 | [crypt32: Use a helper function to allocate signer handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=07ba16c291e3933037f75bb2ca5cdbab7639ff16) |
| Juan Lang | 2007-08-21 | [crypt32: Make a helper function to a free a signed message's handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0080d3d691913577538801696a4b70edc930b4a3) |
| Alexandre Julliard | 2007-08-20 | [comctl32: Create the manifest directory if needed (spotted by Dan Kegel).](http://source.winehq.org/git/wine.git?a=commitdiff;h=4bac1e959dc6a88192abb11ea2aa9cdee1a79b56) |
| Juan Lang | 2007-08-17 | [crypt32: Don't store redundant copy of crypto provider in file store.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9be5007669af733bf9ae81bedfca83eeda5f144f) |
| Juan Lang | 2007-08-17 | [crypt32: Pass crypto provider and appropriate flags when opening PKCS messages, and ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e1108533b98f0c50519eb7dd2227a9c0c3f214a) |
| Juan Lang | 2007-08-17 | [crypt32: Don't store the crypto provider when it isn't needed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d534244702f7c5ca64d707628fd397cbcbb0b8e) |
| Juan Lang | 2007-08-17 | [crypt32: Don't store redundant copy of crypto provider in reg store.](http://source.winehq.org/git/wine.git?a=commitdiff;h=065ed54f690584ee52c46869a755702b4dd0eb05) |
| Juan Lang | 2007-08-16 | [crypt32: Rename a confusing type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f68036cebd370e3d1ccd44df0c3cdf1988e55439) |
| Juan Lang | 2007-08-16 | [crypt32: Where possible, pass a pointer rather than an offset, it's less confusing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f3128c92446663329fac703fff8c6ae24a6c31e3) |
| Juan Lang | 2007-08-16 | [crypt32: Use public type and APIs for memory stores wherever possible.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc37988dff3c8071fdbcb25f84c52f6d39a2d232) |
| Juan Lang | 2007-08-16 | [crypt32: Remove some unnecessary casts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=afc50ce3fe99fef60a1b2a62f6b36efe6fdda238) |
| Juan Lang | 2007-08-16 | [crypt32: Move cert store definitions to header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=adaaab923d1bce88a624b14012d215721cd48408) |
| Juan Lang | 2007-08-16 | [crypt32: Move collection stores to a separate file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9f85156e23c808bc8beff9f32dbfdf2dc7280116) |
| Juan Lang | 2007-08-16 | [crypt32: Move file store to a separate file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71dffcee843fc26f98ed36ed8e38ae2aba2cb1f6) |
| Juan Lang | 2007-08-16 | [crypt32: Use public APIs to empty a store.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6aa10439a9b0dcf28f02097f47b2a9f7ee01abc1) |
| Juan Lang | 2007-08-16 | [crypt32: Use externed vars for context variables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a8aa8787863f688b1e31325ff19fcac2ea3c034) |
| Juan Lang | 2007-08-16 | [crypt32: Move provider stores to a separate file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=131f1d20e717aacf75c5213ae2fbd0d2d880af34) |
| Juan Lang | 2007-08-16 | [crypt32: Move registry stores to a separate file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0070d8226fc1a075b1056abf7596335a654719ca) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipDrawString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f7d27e00202a765ff2f8e6529b616f36d14c32af) |
| Evan Stade | 2007-08-15 | [gdiplus/tests: Added GpStringFormat tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f46b779451ada547ea9ffd6bc8b86eb71c87c214) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipAddPathBezierI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee59d41441bac1a9b797b1385251374c79b55505) |
| Evan Stade | 2007-08-15 | [gdiplus: Handle StringFormatFlagsNoWrap in GdipMeasureString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4107db6bb77b0ad1446f6139dadf8fb3354fdd2) |
| Evan Stade | 2007-08-15 | [gdiplus: Allow null-terminated strings in GdipDrawString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0cead32a64455ec1efd3d37914d948d0b7cbf7a) |
| Juan Lang | 2007-08-15 | [wintrust: Remove redundant check of pbSignedDataMsg (Coverity).](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf3535351ac00e2572388f874fa7d8d47a58f8be) |
| Evan Stade | 2007-08-15 | [gdiplus: Handle empty layout rectangle in GdipDrawString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca949393087e575b2bdefc66bc97bd991516bc7f) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipSetStringFormatLineAlign/GdipGetStringFormatLineAlign.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8c77f9b48db84f4bf65f049cacfb6e29fb1d6cc) |
| Evan Stade | 2007-08-15 | [gdiplus: Use DrawText instead of TabbedTextOut.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be66c3c93b0b4089deaedb75ea658c71af102eb2) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipSetLineBlend stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b56689d22c41a64eb611a5488068e9b89601382a) |
| Evan Stade | 2007-08-15 | [gdiplus: Fix default value of StringTrimmingCharacter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b1237257f086649a204a301c996c29e269a1e7e5) |
| Miko&#x0142;aj Zalewski | 2007-08-15 | [wininet: Support HTTP\_QUERY\_RAW\_HEADER\_CRLF|HTTP\_QUERY\_FLAG\_REQUEST\_HEADERS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ab7d17727c38b3e3acebac1fa4ad10f212a0f7fc) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipMeasureString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a51cf1d35ab635206a2ba3652059a34cc067756e) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipDeleteFont.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a364fc325819db40665c7214558da033af73b470) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipGetLogFontW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=958ece2192c917d24303716b381e9670aac0d20e) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipSetStringFormatHotkeyPrefix/GdipGetStringFormatHotkeyPrefix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=936f310190806eada54edf353c89421cdb0c7b4f) |
| Evan Stade | 2007-08-15 | [gdiplus: Fixed 2 GdipDrawString bugs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=92aa57bece965ff3355bba8cfcfefe8a90699861) |
| Jacek Caban | 2007-08-15 | [mshtml: Call setup\_nswindow on load event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=865d92a6e416b94ed46b73182370b00889c7a5ec) |
| Evan Stade | 2007-08-15 | [gdiplus: Added string format constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=73be69c5760fe882b5fa597cd310f293bd8a13c7) |
| Evan Stade | 2007-08-15 | [gdiplus: Save elements of font's style.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62cae5ab39e31e4ffeb14e3c9495ae25fb247961) |
| Miko&#x0142;aj Zalewski | 2007-08-15 | [wininet: A small test for HttpQueryInfoA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cdfee8153cfe391843486a19f854087d8f39014) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipSetTextRenderingHint/GdipGetTextRenderingHint.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5662820072ef3ce138dd625a08bcd5770d3cee6a) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipGetStringFormatTrimming/GdipSetStringFormatTrimming.](http://source.winehq.org/git/wine.git?a=commitdiff;h=551a606ab247a6a89dc4e1e42c28feb717827990) |
| Evan Stade | 2007-08-15 | [gdiplus: Fixed conformance of font constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=537112fb52a18454eaa5993ec6b4862dd757043a) |
| Evan Stade | 2007-08-15 | [gdiplus: Added more font tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=510ecb653092fada7d1dc09fbdcce000bd2ff9ba) |
| Evan Stade | 2007-08-15 | [gdiplus/tests: Added GdipAddPathLineI test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e041fe4b92e47d097554798e18d3ced81fcc68c) |
| Evan Stade | 2007-08-15 | [gdiplus: Handle empty layout rectangle in GdipMeasureString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44e983925aff41f670be43202055422cdf2aebd7) |
| Evan Stade | 2007-08-15 | [gdiplus: Added font tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4202ababb0b17b368ce9cee3fb180dcb19a3aec5) |
| Miko&#x0142;aj Zalewski | 2007-08-15 | [wininet: Make HttpQueryInfo[AW](http://source.winehq.org/git/wine.git?a=commitdiff;h=3fa49f0f0273345cbe030ab8a45de5176e153007) work for lpBuffer == NULL and len &gt; 0.] |
| Evan Stade | 2007-08-15 | [gdiplus: Handle StringFormatFlagsNoWrap in GdipDrawString.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f32083ed736dd124e9d95d2d53e9d8e074a1a53) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipDeleteStringFormat.](http://source.winehq.org/git/wine.git?a=commitdiff;h=380f18498666bcae9b067c14f331a48513aae48e) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipGetStringFormatAlign/GdipSetStringFormatAlign.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16dea47a5c690d1833547f5740631c558a9def89) |
| Juan Lang | 2007-08-15 | [crypt32: Free default chain engine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1626da2bbaacb5aefc71f9281f025bfd7ccb33c7) |
| Lei Zhang | 2007-08-15 | [riched20: Add missing scroll bar update.](http://source.winehq.org/git/wine.git?a=commitdiff;h=13ae5f8e8c6a5034613874a189ce0625f11dc56b) |
| Lei Zhang | 2007-08-15 | [riched20: Properly calculate control display height.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0d4707c284808df6d87eeb5908df29693889eccc) |
| Evan Stade | 2007-08-15 | [gdiplus: Added GdipAddPathLineI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=059a2d8c6fcfe6007bf3ab7be523f681ab7769ab) |
| Juan Lang | 2007-08-14 | [wintrust: Implement WTHelperGetProvCertFromChain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1ec80d13ba7545ae3278248f776e45ccf2d1ccf) |
| Juan Lang | 2007-08-14 | [crypt32: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1cb8057e71fccfb503d093df99ca686ed3191ea) |
| Evan Stade | 2007-08-14 | [gdiplus: Added GdipSetCompositingMode/GdipGetCompositingMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e807eb9ad6027194114f0f65f87c720a690dd7ae) |
| Evan Stade | 2007-08-14 | [gdiplus: Added font constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d060aeccca03e48c82ff16fc5b2a9d90b9375bb6) |
| Juan Lang | 2007-08-14 | [wintrust: Implement WTHelperProvDataFromStateData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba0b7a5de34ee0873b3e4d2c2065bc1236061a15) |
| Evan Stade | 2007-08-14 | [gdiplus: Better handle UnitPixel pen width.](http://source.winehq.org/git/wine.git?a=commitdiff;h=afa4d3233a073fa76119de0572bf715a5c5e7e56) |
| Juan Lang | 2007-08-14 | [crypt32: Add initial tests for certificate chains.](http://source.winehq.org/git/wine.git?a=commitdiff;h=abd6feaf9350939a6b6886b4ef933a5b83539ab2) |
| Evan Stade | 2007-08-14 | [gdiplus: Added GdipDrawRectangles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d6e0750f25db9f9df34fed6f091c96bda74710a) |
| Juan Lang | 2007-08-14 | [crypt32: Initial implementation of CertGetCertificateChain and CertFreeCertificateChain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a58b30819080a05dfc30914f5e6af34f3089a43) |
| Jacek Caban | 2007-08-14 | [mshtml: Make window.external visible for JavaScript code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=80a1a2f135f493d0d5b5e94b461d2751ef8ff9d5) |
| Miko&#x0142;aj Zalewski | 2007-08-14 | [kernel32: Return error code if WOWCallback16Ex of a real-mode function failed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e79b5656e5fa88e224f118b69c534c3312c38be) |
| Juan Lang | 2007-08-14 | [crypt32: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7316156d35fbf6f75de6486759e8beefc8f2a088) |
| Jacek Caban | 2007-08-14 | [mshtml: Return wine: URI for protocols handled by MSHTML.](http://source.winehq.org/git/wine.git?a=commitdiff;h=718b771f2a57d0c762d24c6ef62f070eb3647e8a) |
| Juan Lang | 2007-08-14 | [crypt32: Set return value on exception.](http://source.winehq.org/git/wine.git?a=commitdiff;h=714a3731eb92261735900e245ae1c91d7bd4c232) |
| Alexandre Julliard | 2007-08-14 | [comctl32: Create a manifest file at dll registration time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6790cdb8f5c8d15df0b19702e36e888c996fc97c) |
| Miko&#x0142;aj Zalewski | 2007-08-14 | [winedos: Make UMB executable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=570eb6093ea0e96e35dc9a23d3de42e2cf166d3f) |
| Juan Lang | 2007-08-14 | [crypt32: Add a chain test with real certificates.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51651c7c5c0c6c086934f1eef13804208129c5ae) |
| Juan Lang | 2007-08-14 | [crypt32: Add stub for CertFreeCertificateChain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=466d8a01a5af51f802ccc6cc5bd1ecfd206a5321) |
| Juan Lang | 2007-08-14 | [wintrust: Forward WinVerifyTrustEx to WinVerifyTrust.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33407c63978c6d801b06f5f9892344e98e0525d5) |
| Evan Stade | 2007-08-14 | [gdiplus: Added GdipRotateWorldTransform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3126c7704ccbd7e3681afc3c1fb182c6f479b740) |
| Evan Stade | 2007-08-14 | [gdiplus: Added GdipScaleWorldTransform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30fdcc7612c539c82567d7925337079223014efb) |
| Evan Stade | 2007-08-14 | [gdiplus: Added GdipCreateFontFromLogfontA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1e33bdcfbd00410b280c4bf513722c10b9637295) |
| Juan Lang | 2007-08-14 | [crypt32: Move CertGetCertificateChain to chain.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1547f39800e6759b9dcc7f092a15c5eb29e73c2f) |
| Juan Lang | 2007-08-14 | [crypt32: Set output chain to NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b2b1f88818c19bb58c26c748e0475aa51e51501) |
| Juan Lang | 2007-08-14 | [wintrust: Implement WTHelperGetProvSignerFromChain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0823c4fc61156540b2c246e334deaccbbe46f23f) |
| Jacek Caban | 2007-08-14 | [mshtml: Check use\_wine\_url in nsIURI::GetAsciiSpec.](http://source.winehq.org/git/wine.git?a=commitdiff;h=000c3d429599bf135a81bc29f6a89383c6294335) |
| Juan Lang | 2007-08-13 | [wintrust: Implement SPC indirect data encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f7e62befe8149fb3f98a4a9789d846263f8c7066) |
| Juan Lang | 2007-08-13 | [crypt32: Avoid a memory allocation when decoding the subject key identifier extension.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f7bcc26cc5f90c9fd58b064247029db8af64a104) |
| Juan Lang | 2007-08-13 | [crypt32: Add missing break.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d49c9d59d1770cd773752277fd874afb47b2c7ba) |
| Juan Lang | 2007-08-13 | [crypt32: Test authority key identifier with a multi-byte id to show that its byte ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b82bfa3455a391c9a9c28fa5b2f47fb1d44d33cf) |
| Juan Lang | 2007-08-13 | [crypt32: Test finding the issuer of a certificate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa0f823429f8a51dcc1d78166c83dc98fab08705) |
| Juan Lang | 2007-08-13 | [wintrust: Implement SPC PE image decoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=998bea104335a04e3f53159abe14ecc1624d0531) |
| Juan Lang | 2007-08-13 | [wintrust: Implement SPC PE image encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d965df2205c6004800c1eb9b6a89e229bb85011) |
| Juan Lang | 2007-08-13 | [wintrust: Implement SPC indirect data decoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=261f02ca68f838ab5fe9013f2ea9d408b9747907) |
| Miko&#x0142;aj Zalewski | 2007-08-13 | [kernel: Allocate global memory with execute permission.](http://source.winehq.org/git/wine.git?a=commitdiff;h=216c3b0d0aee29728adcd8f0b7846563fca030fb) |
| Jacek Caban | 2007-08-12 | [urlmon: Wrap IBindCtx in CreateAsyncBindCtxEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=83a83880cdabe23b655971af45c852ea8c3a0a9d) |
| Jacek Caban | 2007-08-12 | [mshtml: Don't mess with gecko specific protocols.](http://source.winehq.org/git/wine.git?a=commitdiff;h=464121bc003a3ea65c8943bff8eecdd51c5f4235) |
| Jacek Caban | 2007-08-12 | [mshtml: Make get\_typeinfo thread safe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37e386279991f966281f92bdbe6a7c37c5715ecb) |
| James Hawkins | 2007-08-11 | [msi: Add tests for the RemoveFiles standard action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b353a09569d32a8302ffe6278944d9cf4f514b10) |
| Evan Stade | 2007-08-10 | [gdiplus: Better error checking in GdipBitmapLockBits.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff752456e123ded9d77a4654b7889709638a7aaa) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipConvertToEmfPlus stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8b2b77f69bad9d45f3648519d3ed95ab72c9ee8) |
| Juan Lang | 2007-08-10 | [crypt32: Use helper functions to simplify CryptEncodeObject and CryptEncodeObjectEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f848055151c4e9c3db6f8e4cd067f820de4799e4) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipCreateTextureIA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b9411ba374e9570f99bdc23b8769d7ccb64ad1c1) |
| Evan Stade | 2007-08-10 | [gdiplus: Replace GetDC(0) with CreateCompatibleDC(0).](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c30236dee4b0fae1c3be5be23fd5b6002ebd15d) |
| Juan Lang | 2007-08-10 | [wintrust: Add missing definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98dd6c75e29c84a31a2845a1f704afe21cc22fbd) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipSetTextureTransform stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96a69f0508483546f9de505d37200cf656269aa3) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipGetImageGraphicsContext.](http://source.winehq.org/git/wine.git?a=commitdiff;h=94a19d1f759b76de7d2127978a09e844b6026cde) |
| Evan Stade | 2007-08-10 | [gdiplus: Updated GdipCloneBrush, GdipDeleteBrush.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8254c37ad8813442b20d661e07e0bd8b4f6240a9) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipTranslateWorldTransform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=795b62216d6b0a9067e983e84f006c0c6bab2afc) |
| Juan Lang | 2007-08-10 | [wintrust: Add tests for encoding and decoding SPC PE image data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a9d049b74f4a4baa71684069679979d33d2d216) |
| Juan Lang | 2007-08-10 | [crypt32: Validate parameters better in CryptDecodeObject.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d8d9e7d08836698d9f55153cece7c006f7c1751) |
| Juan Lang | 2007-08-10 | [wintrust: Add stubs for SPC\_LINK and SPC\_PE\_IMAGE encoding/decoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c5efcc412c8c05ad2da24f58578bfe5b3cd77ce) |
| Juan Lang | 2007-08-10 | [crypt32: Use helper functions to simplify CryptDecodeObject and CryptDecodeObjectEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c58c4bc2fdb7ad3c7819da55cef005dc63d7e6b) |
| Juan Lang | 2007-08-10 | [wintrust: Add tests for encoding/decoding SPC links.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44047e02c2f1f1497e744664611dccb67ded54b3) |
| Juan Lang | 2007-08-10 | [crypt32: Improve tracing when builtin function isn't available.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a50b1fea64299f57cfb442a11bdbca398cbe840) |
| Evan Stade | 2007-08-10 | [gdiplus: Fix test to pass in Windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2ba471e0d6d5fa5515445e12cf9281905ce37b37) |
| Juan Lang | 2007-08-10 | [wintrust: Implement decoding SPC links.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29cae46fce50cfa059bedca1034fbd82f55a9810) |
| Juan Lang | 2007-08-10 | [wintrust: Implement CryptSIPGetSignedDataMsg.](http://source.winehq.org/git/wine.git?a=commitdiff;h=25f0fb929d8c0fc0bd045906b988079111961572) |
| Juan Lang | 2007-08-10 | [wintrust: Implement encoding SPC links.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06b51457e1622a4f14a3150b96363c2d55e48450) |
| Evan Stade | 2007-08-10 | [gdiplus: Added GdipDrawImageRectRect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=04d4c2621cb31b6d844c021fde10bcdad30c1a06) |
| Juan Lang | 2007-08-10 | [crypt32: Ex encode/decode functions should call non-Ex versions if no Ex version ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=038b53c301364c1775c823b8ad561c494be91413) |
| Evan Stade | 2007-08-09 | [gdiplus: Added GdipCreatePath2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff2e63d41edbc4be10954802946878210c13e599) |
| Evan Stade | 2007-08-09 | [gdiplus/tests: Added GdipCreateBitmapFromScan0 test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cae277f13ed892e731201d941d07da079aaa541c) |
| Evan Stade | 2007-08-09 | [gdiplus: Added GdipSetImagePalette stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c147389ff18f8a5dbc29d40aa35910d8125bffac) |
| Evan Stade | 2007-08-09 | [gdiplus: Added GdipFillRectangle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b66c0a00d9e334c8f732b438978829ab4c550576) |
| Evan Stade | 2007-08-09 | [gdiplus: Added GdipGetPenDashOffset/GdipSetPenDashOffset.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b5d7af5438072f886735f85eff7663a864def089) |
| Evan Stade | 2007-08-09 | [gdiplus: Added GdipCreateBitmapFromGraphics stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad8ea1b0a6054f3ff4873dc983a8ebd0e2c4a6e7) |
| Evan Stade | 2007-08-09 | [gdiplus: Fixed conformance of GdipCreateBitmapFromScan0.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a41fa500f456650a430e7bff817eb306ff14a8cd) |
| Evan Stade | 2007-08-09 | [oleaut32: Handle transparency data when loading PNG images.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a08b998f204374fedfbb73aaa7daf7a18fa2a5ee) |
| Juan Lang | 2007-08-09 | [crypt32: Use real certificates to test finding subject certificates, and correct ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=9da1baa130bf3f414a94f4fa44f097e5e61c20ae) |
| Juan Lang | 2007-08-09 | [crypt32: Correct loading OID functions from the registry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8778b9f506d511c96860f10f9c3f6f37e4dcdd33) |
| Juan Lang | 2007-08-09 | [crypt32: Trace more return values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84a54b5a1f44b029617eaf2b7d92a2643fbeff51) |
| James Hawkins | 2007-08-09 | [msi: Implement the UnpublishFeatures standard action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ac081610966ed3bba1b93f88266da7372e839c8) |
| Miko&#x0142;aj Zalewski | 2007-08-09 | [user32: CallWindowProc[AW](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e9ced90f70cee45f8b66ca578f5bb11b6999e3a) for mismatched built-in winprocs should take into account ...] |
| James Hawkins | 2007-08-09 | [msi: Simplify MsiQueryComponentState, with more tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=511bdd9de8ceade99951d227060ad7fc417a9315) |
| Nigel Liang | 2007-08-09 | [winecfg: Fix crash when remove app button is pressed in applications tab.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f03cf760bf360608b81ba980de7a9a88d71f00d) |
| Juan Lang | 2007-08-09 | [crypt32: Add stub for I\_CryptGetAsn1Decoder.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0c4c1985b0e5e5a818ae1ccae634f5735cfe4a97) |
| Evan Stade | 2007-08-08 | [gdiplus: Updated brush cloner/deleter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ec3049168cb94d587487fa53b1ff14a8a7677f16) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipDrawImageI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=de351ab9917778b95ff38c457e006efccaefe234) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipGetLineGammaCorrection/GdipSetLineGammaCorrection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ddea5bd7bae511b3de0b5c40f707a7e91f4d7efb) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipCreateLineBrushFromRectI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d806c67821ebd2173353c90a43f64d005ed4731b) |
| Evan Stade | 2007-08-08 | [gdiplus: Updated GdipDrawRectangleI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c84c204b48d70b86ee24b6362102d8d98528c274) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipFillRectangleI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb904a277946224da2f13f70ed6edb0d5ff27a5e) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipSetImageAttributesColorMatrix stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a93e61d377f03d390dddfb19b8f8c3a135e71def) |
| Evan Stade | 2007-08-08 | [gdiplus: GdipLoadImageFromStream makes initializations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=985ea4afac506cfa05914bca50f4c135808bee3b) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipCreateBitmapFromFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8726f5ad2dfd68d385ecf2bc69513fe8d295073d) |
| Evan Stade | 2007-08-08 | [gdiplus: Don't prematurely release stream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d03a41325a77c2cc6893e19777e028542f7d6df) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipBitmapLockBits.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a9a30d95c5b26bc93ce1698098d85cd488b4f53) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipSetLineSigmaBlend stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=48ae8ea5422f631277142c4926d1763ec505448b) |
| Evan Stade | 2007-08-08 | [gdiplus: Make GdipGetMetafileHeaderFromMetafile return Ok.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f9fad16923ed3d2e62b20d96b701c4cf35a3b02) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipCreateStreamOnFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ea77f5cfde7dbf1cacf35ff3f0e595eba01d7c7) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipSetLineWrapMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37657bc4d14c4338d0ee64800f8c421f036287b1) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipSetCustomLineCapStrokeCaps stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=369dc8caba29162330981f3eadb931c47164ee0c) |
| Evan Stade | 2007-08-08 | [gdiplus: Added GdipCreateLineBrush.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b438a0220f31e8f1778012f62ba7eff758abfa9) |
| Evan Stade | 2007-08-08 | [gdiplus: Return width and height of metafiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0794e5daf3778495b34617a5d7ce8264069ae1ce) |
| Evan Stade | 2007-08-08 | [gdiplus: Fixed bug drawing custom caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=02887b6c90bd927f23e8ff36ade05ecaf9ab397d) |
| Huw Davies | 2007-08-07 | [wininet: Fix the case when Proxy or ProxyBypass is NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc881a258e0881e1a20417f5dbfdd72535a025e2) |
| Juan Lang | 2007-08-07 | [crypt32: Use the authority key identifier to search for a certificate's issuer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d89528b0161fd3524500aa6bcaac86473ec3631a) |
| James Hawkins | 2007-08-07 | [msi: Implement the MSIINSTALLCONTEXT\_MACHINE context for MsiQueryComponentState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca55c7a3307188952513c01aa8f6abf8da18b46b) |
| Juan Lang | 2007-08-07 | [crypt32: According to MSDN, inner content is only decoded when the content type is ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c9a54102883bab8357993b982c4ef1954c4dcbf2) |
| Juan Lang | 2007-08-07 | [crypt32: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c91e591a95d15c09b994d2d7f25798d7e3e0942e) |
| Juan Lang | 2007-08-07 | [crypt32: Add a couple traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5a213a816379092f76e50dc6602ad03b953c8bf) |
| Juan Lang | 2007-08-07 | [crypt32: Test and correct finding a subject certificate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bcbf5dcee337d83540c188a6572974ead74219cd) |
| Nigel Liang | 2007-08-07 | [winecfg: Fix apply button always available in graphics tab bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e56e37b2d4176912fbc81778c3580c2debb5712) |
| James Hawkins | 2007-08-07 | [msi: Forward MsiQueryComponentStateA to MsiQueryComponentStateW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5f442207d579dc3d6cf5243c4c63c6be966edccc) |
| Juan Lang | 2007-08-07 | [crypt32: Introduce cryptasn debug channel to quiet down crypt traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53087dbe12ea5997c554755107e69c128443fe73) |
| Nigel Liang | 2007-08-07 | [winecfg: Fix crash in graphics tab.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a21ad9f5cb5cf7c7865d27a7f8efd6deece982c) |
| James Hawkins | 2007-08-07 | [msi: Add tests for MsiQueryComponentState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=072adfa99aa0c5ba9e4bbcdb5b6bf4ba2cf692ab) |
| James Hawkins | 2007-08-07 | [msi: Implement the remaining contexts for MsiQueryComponentState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0713c3286934e38704125f3a55748cf03b1756f1) |
| Juan Lang | 2007-08-07 | [crypt32: Implement CertRDNValueToStr for UTF-8 strings.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05d2ab176a83d251c5fd698885ae892e0f971c82) |
| Evan Stade | 2007-08-04 | [gdiplus: Added GdipImageGetFrameDimensionsList stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f3879cd97fd95a3a571f9c98c75450ab436e2fa0) |
| James Hawkins | 2007-08-04 | [msi: Fix the size allocated for the deferred custom action string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1b790be0663790ca9d467737aba2c005306e6ad) |
| Evan Stade | 2007-08-04 | [gdiplus: Allow non-default GdiplusStartupInput.](http://source.winehq.org/git/wine.git?a=commitdiff;h=81c0865bee71f0da14445e139ae7c8c3f868f6cf) |
| Evan Stade | 2007-08-04 | [gdiplus: Added GdipCreateBitmapFromStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8128aeb035ddfa769df99b08ca551eafcc5c007a) |
| Evan Stade | 2007-08-04 | [oleaut32: Allow PNG\_COLOR\_TYPE\_RGB\_ALPHA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72a760beb0595555959e0e45f4a0854dd53869a7) |
| Evan Stade | 2007-08-04 | [gdiplus: Added GdipGetImagePixelFormat.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4d25791b40e5529c5bba30eeecfe960e096171ef) |
| Nigel Liang | 2007-08-04 | [winecfg: Fix crash caused by calling set\_reg\_key with NULL value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4536a9d66d11c46028952de5b44ccf52da43a1b5) |
| Evan Stade | 2007-08-04 | [gdiplus: Added GdipImageSelectActiveFrame stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1015722dfe87266c330097c8c874d8ae356d2b51) |
| Evan Stade | 2007-08-03 | [gdi32: Don't print fixme more than once.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf8b59ef81d448d39204db2fd67972531f92c8e6) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipCreatePathGradient.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b26d7ce82d959026143e128e0c28c110cf43d3b0) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipS/GetPathGradientGammaCorrection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ea7ef468b1911393bf95e3d6359cef3ba9e3a6c) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipG/SetPathGradientCenterPoint.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a9c857b3ffbc21d6fbde0d021daa9b2816373d2) |
| Evan Stade | 2007-08-03 | [gdiplus: Removed old fixmes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=88ab6d32d3597d9e4622092a7e35011c2889293d) |
| Evan Stade | 2007-08-03 | [gdiplus: Use custom cap base inset differently.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f0aa3af7c945a8e538e12eca2b631a44c9c3d06) |
| Evan Stade | 2007-08-03 | [gdiplus: Updated GpBrush functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7929ba8dcecae2a0faaf8b7f7e32c5a4371f5bff) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipG/SetPathGradientFocusScales.](http://source.winehq.org/git/wine.git?a=commitdiff;h=496c319c7001c3429cffda3cf747cf7a66d4b627) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipGetPathGradientPointCount.](http://source.winehq.org/git/wine.git?a=commitdiff;h=490ca1cabb6d0fb75e1829e7e6d9fbd2fa9dccfd) |
| Evan Stade | 2007-08-03 | [gdiplus: Alphabetized header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=46ce55bf99f8ed4670604c10a296f228e1f835fc) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipSetPathGradientSigmaBlend stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15dce3a4324d8f69f9bd8124c09f2b37301910fe) |
| Evan Stade | 2007-08-03 | [gdiplus: Added GdipS/GetPathGradientSurroundColorsWithCount stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=03af4ed338257ffc71018e620c1c23cc5d5c43de) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipIsOutlineVisiblePathPointI stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fdf9f8fb0536d2f56198478e04f2f928f5c22323) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipSetPathGradientCenterColor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2cf5551dbe3453b3701e4a0e20cdb6bb53c251a) |
| Evan Stade | 2007-08-02 | [gdiplus: Added solid-color path gradient brush implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f18cdef727d34d4428d2cef01b151e555f5be25a) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipSetPathGradientWrapMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0dbfe959f9ca0e6faa8c87604525732742c64a9) |
| Alexandre Julliard | 2007-08-02 | [ntdll: Relax the activation context size check.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed3b5322f634a1c75375873ebe7b9191505a8694) |
| Juan Lang | 2007-08-02 | [crypt32: Add CERT\_ID\_XXX defines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7a1e99a763608afe9b7861def2ac33daec953bc) |
| Juan Lang | 2007-08-02 | [crypt32: Test encoding a cert with a subject key identifier extension.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c98f605b0e472a0cd7b19728326abe488e402f26) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipClonePath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bba20a68b8e4895583b917e9df8962d94f4b45bf) |
| Juan Lang | 2007-08-02 | [crypt32: Test and fix getting a certificate context's key identifier property.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac28066b487f5f167f3a26fbced82bf15c6f4d2a) |
| Evan Stade | 2007-08-02 | [oleaut32: Slight correction to EMF rendering.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a55f233219c3877db9defd1c86c4046e869da76f) |
| Juan Lang | 2007-08-02 | [crypt32: Test encoding/decoding a couple more alt name entry types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9194d60061f60577d21313514bc9537c8c43674d) |
| Juan Lang | 2007-08-02 | [crypt32: Add and use a helper function for getting cert properties.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90824039acf6ddf5e328524a4fca4c310945a976) |
| Juan Lang | 2007-08-02 | [crypt32: Implement encoding OID and directory name alt name entries.](http://source.winehq.org/git/wine.git?a=commitdiff;h=676c6e5a3648e65cb1afe7af7b6136f4b384c114) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipDrawLine.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e29e37af5780793e64631670cfcf15ee0b9159b) |
| Juan Lang | 2007-08-02 | [crypt32: Fix typo in key context property test, and the problems it hid.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5885eb3cc3dc38e7933bd5b10ce849c24b238766) |
| Juan Lang | 2007-08-02 | [crypt32: Implement decoding OID and directory name alt name entries.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44948c3b38859cf63a3115b81a7c234a2ca9cba8) |
| Nigel Liang | 2007-08-02 | [winecfg: Remove bad default setting for logpixels registery.](http://source.winehq.org/git/wine.git?a=commitdiff;h=35f4e95c36094372ca03e548ef24abe149c7b7d4) |
| Dmitry Timoshkov | 2007-08-02 | [gdi32: Also print a readable table name in the failure notice.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f71832ac9c5be0929fe0a1e4f6eb6f7905aa0e7) |
| Nigel Liang | 2007-08-02 | [winecfg: Read/write registry in unicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d5a89bab087d09f3e3876e29ae32a2e863273fe) |
| Miko&#x0142;aj Zalewski | 2007-08-02 | [write.exe: Add a new program that calls wordpad.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2777a94d4eef7dd8f8d422bed1c1363a059f9109) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipFillPolygon.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ef7793b51339d37c3f695faa9e90576e8ff5d2b) |
| Evan Stade | 2007-08-02 | [gdiplus: Don't suggest image size when converting WMF to EMF.](http://source.winehq.org/git/wine.git?a=commitdiff;h=192e1115bd9416944ff5fed8c3962271a795cf22) |
| Evan Stade | 2007-08-02 | [gdiplus: Added GdipSetPenWidth.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0d45cd0212365dd66898dbe895ebf18ded265b72) |
| Juan Lang | 2007-08-02 | [crypt32: Support finding certificates by cert id.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cc08cccb92cf974cd50074bed2f652ad7dcce23) |
| Juan Lang | 2007-08-02 | [crypt32: Get rid of bogus check and improve traces for unexpected alt name entry ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cb6148422e455406316ea55cef66adc99c0fd03) |
| Juan Lang | 2007-08-02 | [crypt32: Test encoding a cert with a public key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0c5772dc0a72c8b3e20a60a8d3348c300e83552d) |
| Juan Lang | 2007-08-02 | [crypt32: Introduce a OID decoding function that ignores the tag and use it where ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=005b50e913595892aa0f5832a9f552b67168bd52) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipSetImageAttributesColorKeys stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcbb2111551ee668e88222721190c75dbe9144c8) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipGetMetafileHeaderFromMetafile stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e91d12454a6e709e9e5ded4369ae69f9c3db7455) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipGetMatrixElements.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dd5e9a91f364d02869b00a355227373242d813e0) |
| Evan Stade | 2007-08-01 | [gdiplus: Fix memory leak in GdipCreateMetafileFromWMF.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cfef981a9aeedc7dab3e626aa0aad6b48dcd87b9) |
| Jacek Caban | 2007-08-01 | [shdocvw: Wrong PostData VT is not an error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2395e4907b3df18ec7bc11ced5b054664cedabe) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipSetMatrixElements.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad251e7fe33a3eec2549c69661eb2932f3e1fcfa) |
| Jacek Caban | 2007-08-01 | [mshtml: Release typelib in PROCESS\_DETACH.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a39dec21e2f04c41b5ed5e671136245a367eff44) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipCreateBitmapFromScan0.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9fa4c1248667aa23b88323fbf087e42f547f7ae1) |
| Evan Stade | 2007-08-01 | [gdiplus: Changed GdipGetImageType.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9da6cc907e0bc7e6a09560b9bf6485d61381d5b2) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipRemovePropertyItem stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a0405dc979e1ee9a971d4a0af1fd982bc2f4f83) |
| Evan Stade | 2007-08-01 | [gdiplus: Implemented GdipDisposeImageAttributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d05cb0c4730e0732d574fd8a30c248f0dc0bad7) |
| Evan Stade | 2007-08-01 | [gdiplus: Added partial implementation of GdipSaveImageToStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8304765abdd4e5858149ea0c76b327c2f6d15e6f) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipCreateMatrix3.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7b601148d5ca0e6185fb0602d3f517ce1872e756) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipFindFirstImageItem stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a8866b347f0604d40ec7579921ac197f695120f) |
| Evan Stade | 2007-08-01 | [gdiplus: Implemented GdipDisposeImage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7352cfdb83d72457d0532474215406f67c7538a0) |
| Evan Stade | 2007-08-01 | [gdiplus: Extend GdipDrawImagePointsRect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e0c574fb9ad6f778730a3ae6f74b8d8cbe266af) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipGetPropertyItemSize stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6394e315cf49e4727857214879f64c82269c6bef) |
| Evan Stade | 2007-08-01 | [gdiplus: Track width and height of GpBitmaps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cde960713de02e2864cadc7cadca2e95d37d84a) |
| James Hawkins | 2007-08-01 | [msi: Add tests for joining three tables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f6a93b9c87e930fe6bd5ba16c3e17507dbb1012) |
| Evan Stade | 2007-08-01 | [gdiplus: Implemented GdipLoadImageFromStreamICM.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c5486fe923e138f34f258fff4f8c97c2bae90c5) |
| Evan Stade | 2007-08-01 | [gdiplus: Change include list on 3 tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44412cf1e43bdc212179242ea645129260ed7149) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipCreateBitmapFromStreamICM.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ee25cc3dfbe075a9e0b30df1f30fd75432510a4) |
| Evan Stade | 2007-08-01 | [gdiplus: Added more stubs to gdiplus.spec.](http://source.winehq.org/git/wine.git?a=commitdiff;h=359a21d62bb7bd77c1f84962000ec0fa6930f370) |
| James Hawkins | 2007-08-01 | [msi: Reimplement joins to allow joining any number of tables, each of arbitrary size.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2e6ed06fdcfbb9b71dd550505e784f5d1041eff6) |
| Evan Stade | 2007-08-01 | [gdiplus: Added GdipBitmapGetPixel stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b4b23cfa07f106747de74e1dc20387f0a9b19cc) |
| Evan Stade | 2007-07-31 | [gdi32: Added more tests for ExtCreatePen on PS\_USERSTLYE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff5076c0082d090133be8c8fa1a4bee66e6b9ed8) |
| Evan Stade | 2007-07-31 | [gdi32: Handle PS\_USERSTYLE in ExtCreatePen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eca194da7f733a89fea56a4d6c481710cc1ff93a) |
| Juan Lang | 2007-07-31 | [crypt32: Use the outer content's signature algorithm rather than the public key's ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=e25b81fd9c7679a2bf7bfa632992855655767915) |
| Jacek Caban | 2007-07-31 | [shdocvw: Added GetExternal implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e23c5083f52229cdd0a41b1c532a1f3e4ec641ac) |
| Juan Lang | 2007-07-31 | [crypt32: Remove bad special case, it isn't necessary since the outer content specifie ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=db513c0cb57c1c6e6760562eabf43c69ab750ba4) |
| Evan Stade | 2007-07-31 | [gdiplus: Partial implementation of GdipDrawImagePointsRect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a9c4f30c564a16acf4cc6b543e9882c1f64dccd2) |
| Jacek Caban | 2007-07-31 | [mshtml: Added IHTMLWindow::get\_external implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a84520169f95a9084dec7caea86a929573d819ec) |
| Nigel Liang | 2007-07-31 | [winecfg: Add menu font settings to desktop integration tab.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4d8f32d5521a95264b77f000758704148846a21) |
| Evan Stade | 2007-07-31 | [gdiplus: Added GdipGetImageBounds stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a0b144a1e3b068a6f35c5c121950e8353950d84f) |
| Dmitry Timoshkov | 2007-07-31 | [gdi32: Make GetFontData traces more readable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=991d2d2632e8144c0461004896e8172632719015) |
| Evan Stade | 2007-07-31 | [gdiplus: Added a minimal implementation of GdipCreateImageAttributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d9e4a4a927b622049a5788d31d8c71cae43f24e) |
| Evan Stade | 2007-07-31 | [gdiplus: Added ImageAttributes stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5dd58254843f9841da826076c27421deca8e8ea8) |
| Alexandre Julliard | 2007-07-31 | [ntdll: Load dll from the directory containing the manifest for local assemblies.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b6bb63adbf1eafd7f7fcb0d46fe3e272e1aae68) |
| Evan Stade | 2007-07-31 | [gdiplus: Implemented GdipGetImageBounds for metafiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=586e63ef380335137c83c010b844560d7976d48b) |
| Evan Stade | 2007-07-31 | [gdiplus: Implemented GdipGetImageType.](http://source.winehq.org/git/wine.git?a=commitdiff;h=55c77d46c6ab333daf3349132168dda52f88cfa8) |
| Evan Stade | 2007-07-31 | [gdiplus: Partial implementation of GdipCreateMetafileFromWMF.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50799cf04f1dcc634a6f9f07c39ea06b98f21e65) |
| Evan Stade | 2007-07-31 | [gdiplus: Added GdipDrawImagePointsRect stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=460f01b3208dd0f6e1892d22d40a3105dd26ba86) |
| Evan Stade | 2007-07-31 | [oleaut32: Recognize EMF header when loading picture.](http://source.winehq.org/git/wine.git?a=commitdiff;h=249c07c16104c764481f6701349961998290f418) |
| Evan Stade | 2007-07-31 | [gdi32: Improve ExtCreatePen parameter checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=030abff4ac849df1fcda3ac345cbbdad4ce9575f) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Allow optional elements in the comClass element.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9c9f237635c229750bae29caf0af2eb19308c77) |
| Juan Lang | 2007-07-30 | [crypt32: Simplify alignment calculation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0509c49d1701e9dd962962254226436e9b8ba19) |
| Nigel Liang | 2007-07-30 | [winecfg: Add trackbar to set screen resolution in graphics tab.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e027f0297e378c5ee441fda119b2decdc2585deb) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Convert the XML parser to Unicode to support UCS-16 manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db72af98b556660a699cd6563f9348bd9f86c33a) |
| Juan Lang | 2007-07-30 | [crypt32: Implement getting inner content of a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d6150a7974ed9f2d3e96d674e84189f9bb4c7552) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Fix a compiler warning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b67b66d7b32f3d7014da190d9a449b378331f13d) |
| Juan Lang | 2007-07-30 | [crypt32: Add a few traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a50d8dc1dda877863e1356c36a476bfbbc8f48ec) |
| Lei Zhang | 2007-07-30 | [ntdll: Add Bolivian time zone info.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ee4d8509bcc5a8b675c8e0712bf320180b9c757) |
| Juan Lang | 2007-07-30 | [crypt32: Implement getting the signer cert info from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e10d48c60a36dd266ef3e00f8ee8981278a13c7) |
| Jacek Caban | 2007-07-30 | [mshtml: Added mshtml.tlb registration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d1c59edcee16dbd81fb086fbc2739921f73ece2) |
| James Hawkins | 2007-07-30 | [msi: Treat an empty string and a NULL string as the same value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e81dbebb07fb82131f2e1944797e70b53429b7f) |
| Juan Lang | 2007-07-30 | [crypt32: Separate decoding PKCS signer info into internal and external versions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5900ab1437baacde49c2df1300ae08fdb291a80b) |
| Juan Lang | 2007-07-30 | [crypt32: Implement getting signer info from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=555e85a2b243afa81579c790bb2d0116e0563822) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Use the exact size of the manifest file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53285e2462d2c57e0a590e96ea355983f01751cd) |
| Juan Lang | 2007-07-30 | [crypt32: Add missing definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5270b3233045f751d042ac15b1c762e035e0af3c) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Avoid activation context leak for dlls with no imports.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e4c150bede97661345c67d3ae15eb81f80feefd) |
| Juan Lang | 2007-07-30 | [crypt32: Support getting the inner content OID from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e0f33dada3257373f012a779538bae1b1331b15) |
| James Hawkins | 2007-07-30 | [msiexec: Implement a stub MSIServer service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43bc08ddefec949ea856977e60b01854005fe2aa) |
| Alexandre Julliard | 2007-07-30 | [ntdll: Fixed the null bytes check in RtlIsTextUnicode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43519e415d8712850e51672a189d8a687b5e6c05) |
| Jacek Caban | 2007-07-30 | [mshtml: Added HTMLWindow's IDispatch methods implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4005cf72d6f79404a1df377ecb3379ea5bac5180) |
| James Hawkins | 2007-07-30 | [msi: Add a stub implementation of MsiSourceListEnumSourcesA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37286473a05fb9e35f1ff5e785b675764d10e966) |
| Juan Lang | 2007-07-30 | [crypt32: Test getting more parameters from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2acb8a2dd2e28fa61c73c6c289c5c14d216534b6) |
| Jacek Caban | 2007-07-30 | [winhttp: Added winhttp.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=21572967db5f8b8ba05f791dd0708c9216f46ef6) |
| Juan Lang | 2007-07-30 | [crypt32: Add CryptMsgControl stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=04ef3c05f17d7ee289553ddc2c937869dec61cb9) |
| Juan Lang | 2007-07-30 | [crypt32: Get rid of attribute certs from signed info, they're not supported anyway.](http://source.winehq.org/git/wine.git?a=commitdiff;h=014467031e3a6f18a3c214c2aab1d95ff49584d1) |
| Jacek Caban | 2007-07-29 | [mshtml.idl: Added some missing attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d221915037a8f73cae673b7e19054f83308ffa61) |
| Jacek Caban | 2007-07-29 | [widl: Reorder switch cases to keep alphabetical order.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae0beb224ba12b92b582f5eab31c5f16c5f84cd9) |
| Jacek Caban | 2007-07-29 | [widl: Added displaybind attribute handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8fd971698531aadca65a802ccee225e8192d2c47) |
| Jacek Caban | 2007-07-29 | [widl: Use correct bytes in write\_value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4413e8c6f833f6c7c6ab8b549fb0a13422fd7dcc) |
| Jacek Caban | 2007-07-29 | [widl: Added nonbrowsable attribute handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ad39a38e5a7c46201664c9b09963d9c5df2f133) |
| Jacek Caban | 2007-07-29 | [mshtml: Added mshtml.tlb.](http://source.winehq.org/git/wine.git?a=commitdiff;h=021d06a45fe8802e0c5d04444ceb46e697036866) |
| Juan Lang | 2007-07-27 | [crypt32: A decoded message's parameters are dependent on its type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd1e88ae61aa347e45f32e0770536f46f5e93369) |
| James Hawkins | 2007-07-27 | [msi: Initialize the size parameter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fb45206ed7f99dff600f220b53d7831f375b059c) |
| Juan Lang | 2007-07-27 | [crypt32: Add tests for message stores.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d76e1899ad85e2766b5a55a00eb8b916f6b027bd) |
| Juan Lang | 2007-07-27 | [crypt32: Test getting parameters from decoded signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d187fcd172bb0b5583a93fef7b579cf5b1ce1210) |
| Juan Lang | 2007-07-27 | [crypt32: Implement message stores.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c7f44c8ec7b497e47d46373faaf38946683d4192) |
| James Hawkins | 2007-07-27 | [msi: Implement the MSIMODIFY\_UPDATE command in the SELECT view.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b830fb0a3435a6072ccce407b0605b4742efab6c) |
| Evan Stade | 2007-07-27 | [gdiplus: Check custom dash array for bad properties.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6b7e915c30a83cd5a6dce6606d5f149e4ae1de1) |
| James Hawkins | 2007-07-27 | [msi: Add more tests for MSIMODIFY\_UPDATE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b0ac20e951a65e22836fbc92494770f459545764) |
| James Hawkins | 2007-07-27 | [msi: Keep track of the wildcard record index.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac1f717ab8789cb1288252009aac8821cbcd5918) |
| Evan Stade | 2007-07-27 | [gdiplus/tests: More GdipSetPenDashArray tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a35206e08eb30df1b0be80833ab67f7f8109ff45) |
| Juan Lang | 2007-07-27 | [crypt32: Change type to avoid unnecessary casting.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c7c9e545e2518701e045ff9c47397c7a2ba50fd) |
| James Hawkins | 2007-07-27 | [msi: Use a more unique property separator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9089835c3552d70b1f54901d7e500814a209a9d3) |
| Alexandre Julliard | 2007-07-27 | [ntdll: Simply store the assembly type without interpreting it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f0fb1e3e9830b49ce851aa3748578a8f8a625d4) |
| Juan Lang | 2007-07-27 | [crypt32: Only destroy a decoded message's hash if it's been created.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f2ae254410b36a841d2ca9908e6d4dbd37dc511) |
| Evan Stade | 2007-07-27 | [gdiplus: Fixed a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=629e013d7f25ce06fb7eb48491b781f51efcf7ea) |
| Juan Lang | 2007-07-27 | [crypt32: Store decoded signed content in message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=299612378a9120340ffc8058ddba105bae192a9a) |
| Juan Lang | 2007-07-27 | [crypt32: Correct type of a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=211a8d324f0cdf4e2be1678c5bf8e603be45a2d4) |
| Evan Stade | 2007-07-27 | [gdiplus: Draw custom dashes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f61f4821fb7cd1004b04355306d341a4fc7f216) |
| Juan Lang | 2007-07-27 | [crypt32: Implement getting some parameters from a decoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=115edc67e60308d35c34dd9adeb46ae2f54db39c) |
| Evan Stade | 2007-07-26 | [gdiplus: Added GdipAddPathEllipse.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe2ce3a08b61f5629181148e53d4ec39b58ced1c) |
| Evan Stade | 2007-07-26 | [gdiplus: Fix memory leak.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f52adfd0dea44dcdea0e87b624f9fdf7970d889c) |
| Evan Stade | 2007-07-26 | [gdiplus/tests: Added GdipAddPathEllipse test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e11f7b7bbd5a134bb4077078bbca1ae00c53a9b9) |
| Juan Lang | 2007-07-26 | [crypt32: Add initial tests for decoding signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e0b13a20b5680e797072efd3033a7e10ed32c78d) |
| Alexandre Julliard | 2007-07-26 | [ntdll: Activate the module's activation context while resolving imports and attaching.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e06eaa49ae04444981a92d2aebf590a9d2a1455f) |
| Juan Lang | 2007-07-26 | [crypt32: Test and implement encoding signed messages with authenticated attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5a478edfa98164665d83ba6989aca499910752f) |
| Juan Lang | 2007-07-26 | [crypt32: Test and fix encoding and decoding of attributes in PKCS signers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c58cb379ebf5875ca241b609765554a9099e0e85) |
| Juan Lang | 2007-07-26 | [crypt32: Trace a few more items when decoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8ab462100222dfeece36d123a4478469926f332) |
| Evan Stade | 2007-07-26 | [gdiplus/tests: Added pen dash array tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a8fd94b126f38283d65bf0c88493ef4a3f0837d6) |
| Evan Stade | 2007-07-26 | [gdiplus: Fix arc2polybezier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4f238a1172a84898943353f4f7ab91b7ef9a6fa) |
| Alexandre Julliard | 2007-07-26 | [ntdll: Support single quotes around XML attribute values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f457ac63b8d5324d413126d2453cbf18b942b5e) |
| Juan Lang | 2007-07-26 | [crypt32: Don't check tag in CRYPT\_DecodeDERArray, caller already does.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5674ca2e4e80f30930170fd614c8441088b63ed8) |
| Juan Lang | 2007-07-26 | [crypt32: Test getting the hash from a hash message with an invalid index.](http://source.winehq.org/git/wine.git?a=commitdiff;h=55729020460264338a633d495be305a1aca64400) |
| Evan Stade | 2007-07-26 | [gdiplus: Added GdipSetPenDashArray/GdipGetPenDashArray.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51bd0af43ed168709b8ad489f90075e846d846b3) |
| Jacek Caban | 2007-07-26 | [kernel32: Added a number of activation context tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=43adec3e81f61bbf77f3c1fa4e339c2a1434f391) |
| Juan Lang | 2007-07-26 | [crypt32: Remove redundant assignment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=429e5b300fe88b34f733fad758832ed253ee2e9d) |
| Alexandre Julliard | 2007-07-26 | [ntdll: Improve some activation context traces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b5963c98de2fa36e72df5f2d695f32c8f063ecf) |
| Juan Lang | 2007-07-26 | [crypt32: Partially implement decoding of signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a85fa6b15abe69c6a4a974689a571df41763ea5) |
| Juan Lang | 2007-07-26 | [crypt32: Actually skip content when skipping an item in a sequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30346ee2969125a61460c0ef941311c466343df3) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Check existing dependencies in activation context before adding a new one.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc97dec8d66a5a2002a849e4c454b13debde7a2f) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipDisposeImage stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fba5a59b610c7b1aa658ce597e44ccb148223f24) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipSetWorldTransform/GdipGetWorldTransform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f30732fdf99d7bc0fb13d74ecf0ad6629a378d52) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipCloneMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eab427ee3fc8477df55db652b6334361958523c3) |
| Jacek Caban | 2007-07-25 | [kernel32: Added FindActCtxSectionStringA implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dcbbd30064f87d88132b14eb0acd465d09ad45e7) |
| Evan Stade | 2007-07-25 | [gdiplus: Use world transform when drawing points.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c3e8af414ba653358f4e34cc4b0c3088636b71a1) |
| Evan Stade | 2007-07-25 | [gdiplus: Make pen width depend on world transform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7053b74ba006d5f946051f7dee250ff1271f3e0) |
| Evan Stade | 2007-07-25 | [gdiplus: Limit fixme output.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b0acdb8389f9f52d89075d898d1ed342aa036dad) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Store the base directory for an assembly (based on a patch by Eric Pouech).](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad0d2b90ee7d027d140e4447ea0c2de97e8d30a7) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipGetImageType stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8770b6e8215d98fd0eb31189d639dc8044e3b621) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipLoadImageFromStreamICM stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=875a56ec398a42dd9576ae93b8b753e2f7091bf9) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Don't add an empty assembly when creating an activation context.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82e1aac81d776c203c3e0509f9fb7c7e53921906) |
| Evan Stade | 2007-07-25 | [gdiplus: Added support for more page units.](http://source.winehq.org/git/wine.git?a=commitdiff;h=827f979b37b5e0fb2f0f74c3d5c3acc039c24da4) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipSetPageScale/GdipGetPageScale.](http://source.winehq.org/git/wine.git?a=commitdiff;h=816213955360c650475cddacd117725e968ea8b3) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Use activation contexts information to load dlls (based on a patch by Jacek ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=76bd190a72902d6efab2c85f8aa0d775d02c68da) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipCreateMetafileFromEmf stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cc8c10e0e8930edbba5ec29603a1a17d02131b8) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Fix return status when failing to load the associated manifest for a module.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b844fe84429caaeacb53ebfb13699aedad70ba1) |
| Evan Stade | 2007-07-25 | [gdiplus: Create gdi pen every time gdi+ pen is used.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c424b3c16cf7dc863a36818da8cf209d1543dc4) |
| Evan Stade | 2007-07-25 | [gdiplus: Image getter stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=45c24bbef3e914aaf4ffae5baef896fa2c0db311) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Create the per-module activation context at module load time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4156a716b01c0ebd8ac7dba11806d574fa2eb7f6) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Initial implementation of RtlQueryInformationActivationContext.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a71513d991fe6b818d92eb3c5435b472b216a0b) |
| Alexandre Julliard | 2007-07-25 | [ntdll: Create the process activation context at initialization time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=270f725526ebe3bde8458b8eee44b2ea63cee3f6) |
| Evan Stade | 2007-07-25 | [gdiplus: Added GdipCreateMetafileFromWmf stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=021997fa636391f8b694cec76cba783b1b1b70f4) |
| Juan Lang | 2007-07-24 | [crypt32: Test and implement getting the encoded signers from an encoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f987ca01d0c30481fae09158ff71d4cf15260691) |
| James Hawkins | 2007-07-24 | [msi: Add handling for the MSIMODIFY\_UPDATE command.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4147ca004022228257d3ee89ff1540eb90a0b60) |
| Matt Jones | 2007-07-24 | [kernel32: Added test for bad arguments to SetThreadPriority, test for correct error ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f204ed1d192655d8443437266af937bd91fe11f1) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipGetPenColor stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e43967773f6bb0759433d33910a2da974d9cc4bf) |
| Juan Lang | 2007-07-24 | [crypt32: Add a partial stub for updating a signed encoded message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d11ddebc763bbccb5b07f952085fdb5d342f5ec7) |
| Evan Stade | 2007-07-24 | [gdiplus: Use page unit when drawing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d01c697eb9e721550fb20e751d7763553b4798db) |
| Juan Lang | 2007-07-24 | [crypt32: Add tests for updating signed encoded messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc4005829da1ab4837985fad419de6e3741f4791) |
| Juan Lang | 2007-07-24 | [crypt32: Partially implement encoding signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b80101eb6516e0ac778c1d61bbb26a032ccbd0a2) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipSetPenBrushFill.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a72be4b1676091e779256ff4308f18ed724a8397) |
| Juan Lang | 2007-07-24 | [crypt32: Use consistent types for storing and encoding signed encode data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99c475417a75c0137c86cd1c0e95569493f43d78) |
| Juan Lang | 2007-07-24 | [crypt32: Implement getting outer content of a signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=937b27f3a37e45790a12f790fea9524d399be3bb) |
| Juan Lang | 2007-07-24 | [crypt32: Add tests for getting an encoded signed message's parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c81a386987236250a44786e3390f12f350bbb94) |
| Evan Stade | 2007-07-24 | [gdiplus: Implemented GdipSetSolidFillColor/GdipGetSolidFillColor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b2ce0f94b2097fdcafc6f313b56858a45d2990a) |
| James Hawkins | 2007-07-24 | [msi: Properly delete the columns view.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8a7690c1519189d49d7fc4c6d4a2bd01462fddaf) |
| Juan Lang | 2007-07-24 | [crypt32: Use set encoding function for encoding PKCS signed info.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8a3f4483a9b73ed570b9f6843cea578787431575) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipSetSolidFillColor and GdipGetSolidFillColor stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82abeeea75adf4627fd5143d36434428a01398cd) |
| Evan Stade | 2007-07-24 | [gdiplus/tests: Added pen brush fill test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=777d661fd2bc3eea67896161b0c37dec9de5de28) |
| Juan Lang | 2007-07-24 | [crypt32: Implement getting the hash for each signer of a signed encoded message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71a5859dedcaa774724bd775396f97e1b14d164e) |
| James Hawkins | 2007-07-24 | [msi: Use a different separator as a semi-colon may separate values in the CustomActio ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6af199ef9c4e25e3521f8ad3b109a0ab43edebae) |
| Matt Jones | 2007-07-24 | [server: Only commit SetThreadPriority if new priority is correct.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6763742090f10d953f12d2e4a866f653f89ba529) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipFillPolygonI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6467526469d91f72d05fc3851b797ec5018cb122) |
| Juan Lang | 2007-07-24 | [crypt32: Implement getting version from an encoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f30f90c39bc03b72e98ae00d5ff2767b5b6ee20) |
| Juan Lang | 2007-07-24 | [crypt32: Hash and sign data when updating signed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e2b3ab9e18ad79f47fb568ef2212cbaff9c664c) |
| James Hawkins | 2007-07-24 | [msi: Add tests for the MSIMODIFY\_UPDATE command.](http://source.winehq.org/git/wine.git?a=commitdiff;h=479aca473160842abe99a5e6717a0f3aaabb6dce) |
| Nigel Liang | 2007-07-24 | [winex11.drv: Take into account position of preedit area in PreEditCaretCallback.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f02c27da96d45eb16d3efece4bd0d071fc2c4a4) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipGetPenBrushFill.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37598f81e7c300cf3be10ad321c42c3244a4350f) |
| Juan Lang | 2007-07-24 | [crypt32: Separate signer handles from signer info to avoid unnecessary memory allocation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d359268e60c45903eafecdb42a346c561023379) |
| Evan Stade | 2007-07-24 | [gdiplus: Implemented GdipSetPenColor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=27124d5d327c5fe9a975fd174c47b31bc72d3c25) |
| Juan Lang | 2007-07-24 | [crypt32: Add tests for opening non-detached signed messages, and clarify detached ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=19e63d900484fe49fddbaf02cb872b7a60709a07) |
| Evan Stade | 2007-07-24 | [gdiplus: Added GdipSetPageUnit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=10b575bc8636f262b8667310bbbd96da7d32f040) |
| Juan Lang | 2007-07-24 | [crypt32: More parameter checking for opening signed encoded messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b0df876b2f306d298ca6bc93877cbb3dcd69072) |
| Juan Lang | 2007-07-24 | [crypt32: Test and implement encoding signed data messages with CRLs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=058496451871e29ee705e1536c9c7ada02f215ee) |
| Juan Lang | 2007-07-24 | [crypt32: Test and implement encoding signed messages with certificates.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01ab14e1745ae2630ddd409c822717bed7edec62) |
| Juan Lang | 2007-07-24 | [crypt32: Add tests for signed message encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=014f282b724eeaa8609677c0b621e4f33ea917c6) |
| Juan Lang | 2007-07-23 | [crypt32: Introduce function to encode an array of items as a set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc28f99d22841cd529ec35b3307a5823dd3977ea) |
| Juan Lang | 2007-07-23 | [crypt32: Check for and fail on indefinite-length encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=45652e08029970f6991e0aab7c365eb6b2bb6343) |
| Evan Stade | 2007-07-21 | [gdiplus: Use base inset for custom line caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f56fa321f53e70825b00fc5eeaf71d4e2de4ea95) |
| James Hawkins | 2007-07-21 | [msi: Ref count temporary columns and release them when necessary.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ccef56f2cc6c253eb43fd4e8821456c959f2e908) |
| Evan Stade | 2007-07-21 | [gdiplus: Added startcap rendering.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a84b567cba203a3191e03efcdecd4593e64104ce) |
| Evan Stade | 2007-07-21 | [gdiplus: Added rendering of fill-path type custom line caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c5bcef9f3e5082f00387e49be7f6a56d6557ff6) |
| Evan Stade | 2007-07-21 | [gdiplus: Change atan2 to gdiplus\_arctan2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=818051de2c8769029049ce3d36c6b856f47496c9) |
| Juan Lang | 2007-07-21 | [crypt32: Add tests for opening signed message to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=725d440d3c361df68c16711aa02c96120065e31e) |
| Juan Lang | 2007-07-21 | [crypt32: Add stub encoded signed message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=223bad2312bc22dff601bbe9240ea33afbb36d40) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipRotateMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb478be84cfed37ad2bc6e8466a6b2f3ebee2d9e) |
| Evan Stade | 2007-07-20 | [gdiplus: Use atan2 instead of atan.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea5898c0676634781538be7126c9de4f2c92d616) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipScaleMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d882fc043d83c7888dfa9a81813bb1e008b158d6) |
| Evan Stade | 2007-07-20 | [gdiplus: Initial custom line caps implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d07088ee8ae7c5d05e511c60f3c4280a47aae050) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipCloneBrush.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2b4b87c3b2c6420056f8fd70ea2f01210e1b909) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipCreateMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a8322cb1ad1fc263e8634036dc125827ba2d7cc3) |
| Alexandre Julliard | 2007-07-20 | [ntdll: Don't fail to load manifests that contain unknown elements or attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a24f9cc101ff9d3c983e45953018c383df9b1fac) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipSetPenStartCap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=937432ac176d39d37429017296192d27ba9d7f64) |
| Evan Stade | 2007-07-20 | [gdiplus: Added custom line cap setters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f865f42ee368604b8e5e57ee305b5b19a85d62f) |
| Evan Stade | 2007-07-20 | [gdiplus: Added rendering of custom line caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=85b5df42a792730c4343cbe021d2c69acee90141) |
| Evan Stade | 2007-07-20 | [gdiplus: Associate a brush with a pen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7af2e97a4a4688faf9fec35d02d38cd3193d0af2) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipCloneCustomLineCap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=628237f3344b315b5561681a76a2aedc8d4fa700) |
| Evan Stade | 2007-07-20 | [gdiplus: Updated GdipClonePen to clone pen's members by value, not reference.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5306245c47cc59756497bc826b2292d668f79ae4) |
| Juan Lang | 2007-07-20 | [crypt32: Move decoding hash messages to a helper function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=52cc727348a218ab42c35e3149b68532793ad02a) |
| Evan Stade | 2007-07-20 | [gdiplus: Added GdipTranslateMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=477874797c089172b322b1ba2a2184349645aa9a) |
| Alexandre Julliard | 2007-07-20 | [ntdll: Add support for abbreviated empty elements in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1207d9b5937f7c8fb67d9e4b4843f13c74bea85a) |
| James Hawkins | 2007-07-20 | [msi: Implement adding columns using the ALTER command.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0fd733bf9096d51ef78cba7daafa8a1905bc3ee0) |
| Miko&#x0142;aj Zalewski | 2007-07-19 | [comctl32: tooltips: Remove broken support for non-NULL-terminated strings in TOOLTIPS ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f53e31418006ad899716007b41fbcb9ad409a24d) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Add infrastructure for loading manifest dependencies (based on a patch by ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5bf0947f605cefd9ddfc205e3418d083ce8e8d7) |
| Nigel Liang | 2007-07-19 | [winex11.drv: Implement XIMPreEditCaretCallback.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c52ce9bccc2b6735b73e790f060e31e7544af88b) |
| Jacek Caban | 2007-07-19 | [ntdll: Beginnings of manifest parsing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c0e7cd9d93f1b497db7fcb51d1d0a7c5fe2b1952) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Abstract the entity array type as we need it for assemblies too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b96df32560208c824786a8789ed51c80c931ea38) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Cope with missing assemblyIdentity elements in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2b6fc1288525f290129ed8bfddd886fe090e3cc) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Add parsing of the processor architecture in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5130f4e7280ffed6112f8ebe17eddb46a595ce6) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Add infrastructure for loading a manifest file or resource.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c58a2ce8cca8c83cf37e80f0ad04c664575fe8e) |
| Evan Stade | 2007-07-19 | [winex11.drv: Draw dashed lines for extended pens.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b9e08c2107b31c77692acb5c512d290e36a4259) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Add support for optional flag in dependencies.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84a318265d71d587c50c8168d2950e92e9516acc) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Implemented handling of the per-thread activation context stack.](http://source.winehq.org/git/wine.git?a=commitdiff;h=797dd942ecfc4d405e5e9c3cb528b9698cd79fb3) |
| Juan Lang | 2007-07-19 | [crypt32: Implement querying computed hash of a decoded hash message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74bd61203daca013002c2fef988d846486b5b5c4) |
| Alexandre Julliard | 2007-07-19 | [kernel32: Move activation context creation to ntdll (based on a patch by Eric Pouech).](http://source.winehq.org/git/wine.git?a=commitdiff;h=64f6fdc57e930bbc9a218232bf4804f6872ccb2c) |
| Jacek Caban | 2007-07-19 | [ntdll: Added parsing of the asmv2:hash element in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63e4b943a9ec08172caeb9188d84756326dc74e3) |
| Jacek Caban | 2007-07-19 | [ntdll: Add parsing of dependencies in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5efd2a35bd1d36fec3bb95582d801ed2623bc7a8) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Add parsing of the version in manifests (based on a patch by Jacek Caban).](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b0ab20787e36bf6a7e86a20eb730d69b59510e8) |
| Miko&#x0142;aj Zalewski | 2007-07-19 | [user32/tests: Simplify a test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=46a48c40add87b30daad043dfdb29ee2cb4e16c3) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Move private data to make room in the TEB for the activation context data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44c9758d05a76244b88d13426feb5eff43c69417) |
| James Hawkins | 2007-07-19 | [msi: Implement reference counting for tables, manipulated with the HOLD and FREE ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b1ab76986afccaff08e9b649b42f27b60dd3e33) |
| Miko&#x0142;aj Zalewski | 2007-07-19 | [comctl32: toolbar: Test and fix invalid indexes passed in TB\_ISBUTTON\*.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31be5005c633dee1476a77d93aa27e9c3f628c79) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Skip xml comments in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=272af8fa1eca695182384d8903b532c4a0f6b6f1) |
| Juan Lang | 2007-07-19 | [crypt32: Store hash algorithm ID along with other parameters when decoding a hash ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=22e7c2f38e2303671b3db38b31264c1cab0f1fb2) |
| Alexandre Julliard | 2007-07-19 | [ntdll: Added manifest lookup in global winsxs directory (based on a patch by Jacek ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=214fb6e84e1609b6e61c072719cda4124b667eb6) |
| Jacek Caban | 2007-07-19 | [ntdll: Added parsing of file elements in manifests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16066acf8708716bb7944d53fe56941dccb4fd26) |
| Dmitry Timoshkov | 2007-07-19 | [rpcrt4: Fix the buffer bounds check.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12d3905427796fd65f21673b77381442339ca00f) |
| Jacek Caban | 2007-07-19 | [ntdll: Store the windows directory too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=125e710ff1d620ae8949f08cb22e040ef59c5d83) |
| Juan Lang | 2007-07-19 | [crypt32: Store (most) parameters of a decoded hash message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e90cb9629e1bdfc979ff518b8b333712212e9f7) |
| Evan Stade | 2007-07-19 | [gdi32: Improved PolyDraw in path closed case.](http://source.winehq.org/git/wine.git?a=commitdiff;h=099bfbe1a4e0cd53fc6d22326740eb2356c3953e) |
| James Hawkins | 2007-07-19 | [msi: Add more tests for the ALTER command.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0169533be8d0a4f000e2cd264d04d1e71c19408a) |
| Huw Davies | 2007-07-19 | [wininet: Stub for InternetQueryFortezzaStatus().](http://source.winehq.org/git/wine.git?a=commitdiff;h=00631b24805faa445d321058963380a4486d07c7) |
| Huw Davies | 2007-07-18 | [wininet: Certain options of InternetQueryOption can take a NULL handle, so don't ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d9bdf793fe32a69ef29aa40096b410a4a3c67d02) |
| Juan Lang | 2007-07-18 | [msi: Return FALSE from MsiGetMode for MSIRUNMODE\_OPERATIONS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=955f5f3910a12fcc3e95983e3e46c079b45b5d23) |
| James Hawkins | 2007-07-18 | [Revert &quot;msi: Only call a custom action remotely if the type is msidbCustomActionTypeI ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=929acbcb7f019d89101c579e0348bc3ad5120a7e) |
| Juan Lang | 2007-07-18 | [wincrypt: Add more missing definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=834dbceadaacd45514865a99369f9fdee8fdb070) |
| Evan Stade | 2007-07-18 | [gdiplus: Added GdipClonePen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=628c9a69c1ee6b2321d81866eab299aca03e95eb) |
| Huw Davies | 2007-07-18 | [wininet: Stubs for IsUrlCacheEntryExpired[AW](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f2d93b51260fde45ca5e252044ab066d4acaead).] |
| James Hawkins | 2007-07-18 | [msi: Only double the size if the remote call is from MsiGetPropertyA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=24e158e972e03c992389c259d05ab41ad1dcc1b5) |
| Evan Stade | 2007-07-18 | [gdiplus: Added GdipMultiplyMatrix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12e3eadd415a13c070673234fc97817ca53a704d) |
| Evan Stade | 2007-07-18 | [gdiplus: Added GdipGetPenDashStyle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=024800cb9abc22e3a11749e76ee1c7eca8aa854c) |
| James Hawkins | 2007-07-17 | [vdmdbg: Add a stub implementation of VDMEnumTaskWOW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2fc4d3a0f98754ac258d1e447f06d91c070cc07) |
| James Hawkins | 2007-07-17 | [msi: Only call a custom action remotely if the type is msidbCustomActionTypeInScript.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2ae31000b6d6c105838fad36c17ba1fb1f5524b) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipPathIterCopyData.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef6c41663159c38eba19a166773c5b871ef5ec25) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipSetPenDashStyle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=daf00ab72a2b2e3a3a87f93ea312133ab4ab4ce9) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipSetPenMiterLimit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d59fe31e8b498fbe540bd101143e5bac985709a9) |
| Juan Lang | 2007-07-17 | [crypt32: Fix typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c59d51ab24b5b508ca00fbc4c66ba82dfb9a3ef0) |
| Evan Stade | 2007-07-17 | [gdi32: Added PATH\_PolyDraw.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96937e04a24d7e27b1bd2e97a730b67ad4ef2385) |
| Juan Lang | 2007-07-17 | [crypt32: Add a few tests for decoded message parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=95bb1be2b72515c2c7dfa2dfd4f57fdd3f3e065b) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipPathIterNextSubpath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90ff0fdd6c813a762fd490aee9a369146243c014) |
| Juan Lang | 2007-07-17 | [crypt32: Use property list for decoded message parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8df323f84a8d22fea63ee565065096cf67fd5f1d) |
| Juan Lang | 2007-07-17 | [crypt32: Remove a redundant line.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8cf82d8a0e7a6278a9a49294bb051f3c0664592d) |
| Juan Lang | 2007-07-17 | [crypt32: Fix a bad comment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8099ff4bced2f5c7bf84d17150a503840899ae02) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipAddPathBeziers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e1917852968c61f964d055fa1c69df55ab222d9) |
| Juan Lang | 2007-07-17 | [crypt32: Move digested data encoding to encode.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=703a0f6fce49553fd66bc120f1d5128ea5250ead) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipSetPenLineCap197819.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6893ef397ba63205bd102c5b262c943684fdf911) |
| Juan Lang | 2007-07-17 | [crypt32: Add tests for decoding a hash message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60c6a9e3816822f481ba5383a64a21215f283326) |
| Evan Stade | 2007-07-17 | [gdi32: Added PolyDraw tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=578ff168b366a9248e8662e5c06c0f5ae3713441) |
| Juan Lang | 2007-07-17 | [crypt32: Implement getting content of a data message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e2894493414da24429f557ae307791592ca216a) |
| Juan Lang | 2007-07-17 | [crypt32: Implement decoding hash messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=35abf3adf3d7daa0914df8d57c19fbaea2a00547) |
| Evan Stade | 2007-07-17 | [gdiplus: Export GdipSetPenLineJoin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=18ee93b0c4826e3f23577f0ad25855e1659bb068) |
| Evan Stade | 2007-07-17 | [gdiplus: Added GdipPathIterRewind.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1182162dac3dd31e7ec47608b54200b9072062b8) |
| Evan Stade | 2007-07-17 | [gdiplus: Initial path iterator implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=085082897a47fec1113fad66b38d2129c1123acc) |
| Juan Lang | 2007-07-17 | [crypt32: Add a couple more parameter tests for hash messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=056b4f10dd0c7dd44457cc2115b6b8436edf903b) |
| Dmitry Timoshkov | 2007-07-16 | [shell32: Add a cache for queried shell folder interfaces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f686cfab2feb9010efe82a932dc9f5904566c8ab) |
| Huw Davies | 2007-07-16 | [kernel32: Overlapped pipe tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e59a947c8860a07db11b047a75d897d2a0007217) |
| James Hawkins | 2007-07-16 | [msi: Load the AdminProperties stream if the package is an Admin package.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc3060c542661173937d3aa948f51ced7bbbdd5b) |
| Evan Stade | 2007-07-14 | [gdiplus: Added pixel offset mode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d6bd866df5ec0f4b253af14d677348967cc89138) |
| Evan Stade | 2007-07-14 | [gdiplus: Added GdipFillPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d362b58ded69e08ae4ee20d21b238889b5f3ee0d) |
| Evan Stade | 2007-07-14 | [gdiplus: Added GpGraphics save/restore tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d13e1ba0e826a3acd59497978c98c150b24b8532) |
| Evan Stade | 2007-07-14 | [gdiplus: GdipSaveGraphics/GdipRestoreGraphics stubs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c760668cabb5a9f17a728bbfdb9fbb838a1e7a5b) |
| Evan Stade | 2007-07-14 | [gdiplus: Added interpolation mode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a87ce7ab9265f4b90d34f48dae1474e72330fbc2) |
| Evan Stade | 2007-07-14 | [gdiplus: Simplified GdipDrawPath by moving more of the code to the helpers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e88347f4533a67df0b9cb119314b7cf5a8d4a8b) |
| Evan Stade | 2007-07-14 | [gdiplus: Added GdipSetPathFillMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68a3d94722fba2a7f245a2014d70aec424d8c99c) |
| Evan Stade | 2007-07-14 | [gdiplus: Added compositing quality.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60cad2352230b588a7d3bdd62a0048cdfaad0721) |
| Evan Stade | 2007-07-14 | [gdiplus: Added smoothing modes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53e17d2993f51b9fa8079ad5df6a1ff93d1955e7) |
| Evan Stade | 2007-07-14 | [gdiplus: Constructor tests for GpGraphics.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05a7cef855331d8653ed528d88bfa26b50273ca9) |
| James Hawkins | 2007-07-13 | [msi: Fix three tests that were failing in Windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed281b725aeaab3df51e8f6b438758878248b6f3) |
| Evan Stade | 2007-07-13 | [gdiplus: Use passed pen in GdipAddPathWorldBound.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e547ceb1f65e3367b0e665f71cd218355300f57a) |
| Evan Stade | 2007-07-13 | [gdiplus: Added GdipResetPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d174bcc8a6955d1ad5f9493e1de679b0be89beee) |
| James Hawkins | 2007-07-13 | [msi: Fix automation.c compile for MSVC.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c7b53d37e15487ca7cd1fe141f4bcbde36c7c846) |
| Evan Stade | 2007-07-13 | [gdiplus: Added GdipAddPathPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c41a77a358abeba54a629b87a1e4caed5db584d9) |
| Evan Stade | 2007-07-13 | [gdiplus: Added GdipSetPenLineJoin.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bcd0eda68701150fa98624d8b10fb1a221c7273a) |
| James Hawkins | 2007-07-13 | [msi: Add a test for installing from different current working directories.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba257f0ceac03397702d75e3404408b0d692d71f) |
| Juan Lang | 2007-07-13 | [crypt32: Fix decoding sequences with extra trailing data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8dcd9e4279ef6601440b92fd94a30e046be589da) |
| Juan Lang | 2007-07-13 | [crypt32: Implement decoding data messages (when opened in non-streaming mode).](http://source.winehq.org/git/wine.git?a=commitdiff;h=76061f403b0a2491803259ef30293fcdfa6a2d7d) |
| James Hawkins | 2007-07-13 | [msi: Fix compilation in MSVC.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c940b9b49c7d2755b85c0fe265ec30aec1cf9a2) |
| Juan Lang | 2007-07-13 | [crypt32: Store crypt provider in decode message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a07ca44420076056467742f780b445b91fd0af4) |
| James Hawkins | 2007-07-13 | [msi: Add a test for running an ADMIN install.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6805bf8acee22af3d3e7260229b3309d812b7d7b) |
| Evan Stade | 2007-07-13 | [gdiplus: Added GdipGetPathFillMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=64035b308e978f03796cf5cc7e28fd3460889cd4) |
| Evan Stade | 2007-07-13 | [gdiplus: Added GdipAddPathPath test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44691eefb452e5fdec54f87ca98413f9c90b3fc6) |
| Evan Stade | 2007-07-13 | [gdiplus: Added more GdipGetPathWorldBounds tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41a9a838909d94e9e095748a3fb8437bfe495544) |
| Evan Stade | 2007-07-13 | [gdiplus: Improved GdipGetPathWorldBounds handling of both matrix and pen's effect ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3dc17d2544570eb8db63fb2ac452318e1180bd3d) |
| Juan Lang | 2007-07-13 | [crypt32: Partially implement updating decode messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2cca297ba657c9ee03a1a7d271a4a0a4b6f599e3) |
| Juan Lang | 2007-07-13 | [crypt32: Add test showing extra trailing bytes should be tolerated in encoded data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01685bca0e3a5eedfda8f5b18a4f769b5450dffa) |
| Juan Lang | 2007-07-12 | [crypt32: Copy data in hash message update.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fef57dad46893908e4bf956bb5ad4f13340c72f4) |
| Evan Stade | 2007-07-12 | [gdiplus: Added draw\_polybezier error checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa31217d6e831bf7b04f05d42e0c3dd58f496979) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipGetPathWorldBounds test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9b0dac9f55ed876a0438450b3140e4f551870a8) |
| Juan Lang | 2007-07-12 | [crypt32: Don't check if msg is NULL, tests show native doesn't either.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f83da5cc0757a67b1e5fe3726014330774efdd69) |
| Evan Stade | 2007-07-12 | [gdiplus: Added basic matrix implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f28262b47da30f5d660bdc37244da81d4c3e1240) |
| Evan Stade | 2007-07-12 | [gdiplus: Fixed memory leak in GdipDeletePath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e9eceb5f313180e6bf9a5b893df9a9e64cbb9a5d) |
| Juan Lang | 2007-07-12 | [crypt32: Test opening hash messages to encode with streaming.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e6c339d076e38d169e042306519db4c1ae7b58e7) |
| Juan Lang | 2007-07-12 | [crypt32: Add more missing defines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e3d6f771e85792833e96c57d8a05ad53405e3980) |
| Juan Lang | 2007-07-12 | [crypt32: Update comments about hash message version numbers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1bd2ea907bb8d80b324794715416447d4dccff3) |
| James Hawkins | 2007-07-12 | [msi: Fix a copy and paste error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf3f442754cf3faca81d23186e6dc83eabed1370) |
| Juan Lang | 2007-07-12 | [crypt32: Simplify hash value tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2f8191a648621f41831fb7e30c6898c5e994153) |
| Juan Lang | 2007-07-12 | [crypt32: Implement getting a hash message's hash value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bb1246a51c5c8509ebfbcca324b7ad907739a67f) |
| Juan Lang | 2007-07-12 | [crypt32: Add open tests for hash messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b12072b72d7fad907ae204ca6bb0423f092aa840) |
| Juan Lang | 2007-07-12 | [crypt32: Implement streamed encoding of definite-length data messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=afaba37ed71ba3d4fc15cb7fb0d47f8ba869da00) |
| Juan Lang | 2007-07-12 | [crypt32: Add tests for updating hash messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad975f672bf713da7c2af4d97f4ca68f191ca2c8) |
| Juan Lang | 2007-07-12 | [crypt32: Introduce an updated state, and use it to remove boolean &quot;begun&quot;.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a8e135f4c6b39ea6e0c4cee846815fb23333eeec) |
| Juan Lang | 2007-07-12 | [crypt32: Add a helper function to copy params.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a468e6f6c3be2d7de4c55e79ff7fe9f7fc16f870) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipDrawPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d5f568183340e53e82fb623fed0d04490f66112) |
| Juan Lang | 2007-07-12 | [crypt32: Relax a test, the specific error isn't so important.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9bdb084eb6945d349fcde825629c7a67ea18b9af) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipStartPathFigure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8a76d1e82c6c39ca946f42d01b6875cceb737002) |
| Juan Lang | 2007-07-12 | [crypt32: Add tests for retrieving the content of a non-finalized (detached) message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=880507d9069365317a2b7fc7435e8907b3af911f) |
| Juan Lang | 2007-07-12 | [crypt32: Implement retrieving a hashed message's content.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8599fd77487c9aa7c4a7fbda244a35fe953efc6f) |
| Evan Stade | 2007-07-12 | [gdiplus: Updated GdipDrawLines to use SaveDC()/RestoreDC()/end caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=852aac8b54b12812187d5c4dc558b5fb52cbcc07) |
| Juan Lang | 2007-07-12 | [crypt32: Implement getting hash message version.](http://source.winehq.org/git/wine.git?a=commitdiff;h=804b9d71656d1b478dc1b2ffad62a65e04b1e618) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipGetPathWorldBounds.](http://source.winehq.org/git/wine.git?a=commitdiff;h=78510e70e76e8fe40a292c9dde79a4f1fa2f45f3) |
| Juan Lang | 2007-07-12 | [crypt32: Partially implement updating hash messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=739cc08b3bb95b7f5a320c946f2ecb002e734f36) |
| Juan Lang | 2007-07-12 | [crypt32: Add tests for hash message encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72b8f8325f5df78f350137b7189281ef870edbd8) |
| Evan Stade | 2007-07-12 | [gdiplus: Added draw\_polyline error checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f4ab5282411cde3298fa1c036004f2894350d73) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipAddPathArc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69fa7457e5d746b71c8fef1f2ffb1924a5bc8d35) |
| Juan Lang | 2007-07-12 | [crypt32: Introduce an algorithm id encoding function that encodes missing parameters ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=678fb8ac14b3062a3221247f66075c5ca02862de) |
| Juan Lang | 2007-07-12 | [crypt32: Test updating hash messages with NULL stream output function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cb26d8e58b0640abccec28b3ee649c9bed6cdeb) |
| Evan Stade | 2007-07-12 | [gdiplus: Changed the way the direction of the endcap is calculated to make LineCapArr ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=55d70e894cd70f69d313771e8f5dedd56cce4bc0) |
| Evan Stade | 2007-07-12 | [gdiplus: Moved two inline helpers to the header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a8a1b423c4d8984e61eae9efff7cbdf846b79f1) |
| Juan Lang | 2007-07-12 | [crypt32: Make some encoding functions available outside encode.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=48afa16386c47a27b9b230dfb726959418c9d28a) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipTransformMatrixPoints.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47a605ef9bd2bae60ba74d5f60a2bd1792dfab9e) |
| Evan Stade | 2007-07-12 | [gdiplus: Updated GdipDrawArc to use SaveDC()/RestoreDC()/line caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=40f2273f0354ce403684623449379a0da388e98a) |
| Juan Lang | 2007-07-12 | [crypt32: Detached hash messages don't contain the content, so don't make a copy of it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ffb4b1c4871011631a1d580fd77aa0e5fc7cbb8) |
| Juan Lang | 2007-07-12 | [crypt32: Add a stub hash message implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c15f98b77d9f1f9dd671b16c8b0e8744a8b241c) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipTransformMatrixPoints test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=37d91b04f3b7abf2c6876c75d7e3e0bfdd422dd2) |
| James Hawkins | 2007-07-12 | [msi: Reload properties as they may have been changed by a transform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30fc5602def216483177150160bd45c90fb20d64) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipAddPathArc test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f7cfb1dc829bcec72b3af324ef4c125cd82de91) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipTransformPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f1ecfb2b51bb0cab790c9c83cd8cbd8fb20d013) |
| Juan Lang | 2007-07-12 | [crypt32: Add tests for getting hash message params.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1745d8a7285a9555ef3617c96fadc8b4c8dadb25) |
| Juan Lang | 2007-07-12 | [crypt32: Change finalized from a boolean to a state and use it to simplify message ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=09c4faf159c1a6897926ea559f687aa552b26d46) |
| Evan Stade | 2007-07-12 | [gdiplus: Added GdipCreateMatrix2 test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05450b036611a8b7c5b5430bf89389dd397dda41) |
| Huw Davies | 2007-07-11 | [kernel32: Swap incorrect use of buffers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f2894533d561bb1c42872e54eef9599251e450d7) |
| Lei Zhang | 2007-07-11 | [winex11.drv: Remove old dnd code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0e068744a02c6a66685aec8db72a23db9d05962) |
| Juan Lang | 2007-07-11 | [rsaenh: Get rid of the hash idle state, native doesn't behave as though it has one.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cd3954e7fdeda223b81524a1f41839af90408b31) |
| Evan Stade | 2007-07-11 | [gdiplus: Changed calls to floor to floorf.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6544d9ee3e149234991406f188b357dd0d9d253b) |
| James Hawkins | 2007-07-11 | [msi: Fix current \_Property table tests and add more tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a8e0e8c1dad256c1b47885b889e63472879d516) |
| Miko&#x0142;aj Zalewski | 2007-07-11 | [msxml3/tests: Avoid a crash that happens on some native systems.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c29359286f2e0db5559862ef1c15cc679ce2607) |
| Huw Davies | 2007-07-11 | [kernel32: SetNamedPipeHandleState() is a stub, so for now don't check its return ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=154389ce8e98f2f1639c3d03490174ec170a2d34) |
| James Hawkins | 2007-07-11 | [msi: Add tests for adding properties in a transform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1093eb83cd37c57895154afe21706333421fcae8) |
| James Hawkins | 2007-07-11 | [msi: Add tests for adding properties with a transform during an install.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f6aaf86bd52ec382bc6ecb7982e7701e484c553) |
| Evan Stade | 2007-07-10 | [gdiplus: Added constructor and destructor test for gdiplus paths.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fec9e5e8031ba35e840ad2804027e29d4d2b9c5f) |
| James Hawkins | 2007-07-10 | [msi: Check for NULL transform, as there may be no transforms for the \_Columns or ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f0b97cb1e175eb82fc05821f5e72d9181f046989) |
| Miko&#x0142;aj Zalewski | 2007-07-10 | [comctl32: toolbar: The iImage in TBN\_GETDISPINFO should be initialized to -1.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e66523e19bf17f4b12852ce6d8168a21159fb139) |
| James Hawkins | 2007-07-10 | [msi: Match the changes made by the hand-generated and API-generated transforms.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dfa1b1299cbdea6f22016d03788532abb65718e7) |
| Evan Stade | 2007-07-10 | [gdiplus: Added a test for GdipAddPathLine2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da23ed6e0f95893b069f0f0ede16002a0970c31c) |
| Evan Stade | 2007-07-10 | [gdiplus: GdipDrawCurve2 now uses SaveDC()/RestoreDC() and end caps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b72dc0df9d534322b74efa493d6e73793cc20f62) |
| Evan Stade | 2007-07-10 | [gdiplus: Updated draw\_pie to use SaveDC/RestoreDC.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4fff71454ac04b7b3aa4f4a8f1dbf41505b1617) |
| James Hawkins | 2007-07-10 | [msi: Test adding columns with data in a transform.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9285351ad3b088ff126fde7f62648348682c4d40) |
| James Hawkins | 2007-07-10 | [msi: Delete msifile after the tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5af06dec83870d73ba0234ec25e97a8a7fdb8385) |
| Miko&#x0142;aj Zalewski | 2007-07-10 | [comctl32: toolbar: We should send TBN\_GETDISPINFOW even for ANSI controls (with testc ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5507a073c5e1be9101440c110d2d1e7092a4d293) |
| Alexandre Julliard | 2007-07-10 | [winedump: Add RT\_MANIFEST resource type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4da30bfcfc7607bb4ddd057900120092fd46786c) |
| Alexandre Julliard | 2007-07-10 | [include: Add some definitions for manifest resources.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41db95323d67cae850f6d35ee1ffba16bc0da349) |
| Lei Zhang | 2007-07-10 | [start.exe: Put double quotes around arguments with spaces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30a22664e66f8625522e734741979977c6f54e7b) |
| Evan Stade | 2007-07-10 | [gdiplus: Make LineCapArrowAnchor look more like it does in windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30084db2ce2ba20800610726954533eddb9abcc7) |
| Evan Stade | 2007-07-10 | [gdiplus: Fixed bug in GdipGetPathPoints().](http://source.winehq.org/git/wine.git?a=commitdiff;h=1fc841f6555d9700499dcc59adf0e6b1d6bc5795) |
| Juan Lang | 2007-07-10 | [crypt32: Implement CryptSIPLoad.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19c3a09ba8160c3b654f39681f6abdc550ab5d39) |
| James Hawkins | 2007-07-10 | [msi: Handle adding columns in transforms.](http://source.winehq.org/git/wine.git?a=commitdiff;h=17ba74195bec3d384539249a4bf7de659121041e) |
| Evan Stade | 2007-07-10 | [gdiplus: Updated GdipDrawRectangleI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14e0df1fa0c0225d8de4d997b64aaec74963dd9a) |
| Evan Stade | 2007-07-10 | [gdiplus: Fixed a bug in helper function draw\_polybezier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14c7466c9f2d726741e9e9f9cf6a8befc527a147) |
| Juan Lang | 2007-07-09 | [crypt32: Add more tests for opening a data message for encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd05fe0d132a503b00aebd263aab46e63ddcfaa7) |
| Juan Lang | 2007-07-09 | [crypt32: Test and fix CryptMsgGetParam for streamed messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e557d36320bad7768271e1774bb3e9acbb7bc8c2) |
| Juan Lang | 2007-07-09 | [crypt32: Pass function pointers to CryptMsgBase\_Init rather than rely on callers ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc63bf2de396cfa3db64a13f8bc54fda9075b2fb) |
| Juan Lang | 2007-07-09 | [crypt32: Add tests for streamed encoding of data messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b18b05f53c08ae1ffc87c83447b9e562ea6bacd0) |
| Juan Lang | 2007-07-09 | [crypt32: Add some tests for updating decode messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=acc0bec41ff75632442e38725e86a20f884e57fd) |
| Juan Lang | 2007-07-09 | [crypt32: Test that inner content OID is ignored for data messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aa99cf8ec04801945f4c11f880f6fe64ec6c9dc8) |
| Juan Lang | 2007-07-09 | [crypt32: Implement getting the type of a decode message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ca755915b6f677d51837b5e00658617474bd68e) |
| Juan Lang | 2007-07-09 | [crypt32: Make a copy of a passed-in stream info rather than assuming the pointer ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e65d9439cd0141459cf3f0f3e1553c66518a71c) |
| Juan Lang | 2007-07-09 | [crypt32: More decode message update tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=685d7e799a84dfa51e79e56594a4bd1107403a0b) |
| Juan Lang | 2007-07-09 | [crypt32: Add a stub decode message implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=656d960dd4b01e1ef1f293e1214f8b1629c7c2e6) |
| Juan Lang | 2007-07-09 | [crypt32: Implement CryptSIPGetSignedDataMsg, CryptSIPPutSignedDataMsg,](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d5a8b2f781e2a4a8894c84d2590a8e198a24cea) |
| Evan Stade | 2007-07-07 | [gdiplus: Rendering of linecaps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5128e5dc58c7e2d0f6c8550a06a38337604661b6) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipAddPathLine2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4118c1847e750ccfcd8059c6ff009f43233ea7e) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipClosePathFigures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0ba8711ff24ee59df9d87423ddb5b85f8c93186) |
| James Hawkins | 2007-07-06 | [msi: Handle remote calls to MsiFormatRecordW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cba1b1e1f480cecc6e3bca4fe2978efb2585a800) |
| James Hawkins | 2007-07-06 | [msi: Forward MsiFormatRecordA to MsiFormatRecordW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba4919912c0087ea614f0f55d31c7dfcdd809427) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipClosePathFigure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c1291974450850de52f07f66f56a5597929955e) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipGetPointCount.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8a114adefe34e2ded326094a7087c13547648cea) |
| James Hawkins | 2007-07-06 | [msi: Handle remote calls to MsiEvaluateCondition.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6b97f8905dc9435b8018a297472b4f4dbec315a3) |
| Evan Stade | 2007-07-06 | [gdiplus: Added linecap rendering for GdipDrawBezier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69a807c6a9a5729c1c8458f92a7ac39754287572) |
| Evan Stade | 2007-07-06 | [gdiplus: Added SetPenEndCap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68ba30f4333ac468b04656016fc7355ab0bfb2e8) |
| Evan Stade | 2007-07-06 | [gdiplus: Public declaration of GdipSetPenEndCap.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5dc8dee76d21957b72d89ff6299b84f34d96b56c) |
| James Hawkins | 2007-07-06 | [msi: Fix use of BSTRs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29ce520df98005c8b6e74145a9097b3020e91872) |
| James Hawkins | 2007-07-06 | [msi: Enable remote custom actions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1647de570bedb0052359075367e49dbae5ecc7b6) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipGetPathPoints.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08784f371762133fb57a6329926345899856d3cb) |
| Evan Stade | 2007-07-06 | [gdiplus: Added GdipGetPathTypes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06206fc4a5a8cbfa31b40fa570f2572f06c27217) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiSetTargetPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f935e94adffcdf834972a1ca21649854fcbb05e3) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiSetFeatureState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f45b3ce60e4282d239b9e5396ed180af41557390) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetMode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c96f1d524b50d4a1506c5ce4c25f8e624221f617) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiSetInstallLevel.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c6741d83c6476a7862c148f8ad2cb5acd27563a3) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiProcessMessage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be5eec45b5f68aab9469bfc70602ec554e8057f1) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetTargetPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7479be1bb24257533447bbae049cc13d41bfdc8) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiSequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99714f12cb08fb40521f6d8e12fab2ca7a40b622) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiSetComponentState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82b0066f706631425d76fa15d8c5784ab29e8044) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetFeatureState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d93e1a2a5a782f10c5d36d11724584b06fe5dc5) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetSourcePath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=582be6a73a11a6bc3b47fc9c7da73c14aa0c0a9b) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetLanguage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=569ea392a7ccc5ced3e4b6fd96ffdc10d04e4c00) |
| Evan Stade | 2007-07-04 | [gdi32: Don't access DC in PolyDraw after releasing handle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53e05015f6d5bfb6c2418775688143c7894b4459) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiGetComponentState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=254e27ad31dfb0e34b5474cd831baf73eef2f5c8) |
| James Hawkins | 2007-07-04 | [msi: Handle remote calls to MsiDoAction.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0f321c0af9503219ab8667ce0a84bb75d38fc602) |
| James Hawkins | 2007-07-03 | [msi: Add the IWineMsiRemotePackage interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9001058b07b9d77b447ef3dbfee0ee5774a16c6) |
| James Hawkins | 2007-07-03 | [msi: Handle remote calls to MsiGetActiveDatabase.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4658e05f2a930caef6d1c45e3605e49503b12bf) |
| James Hawkins | 2007-07-03 | [msi: Add tests for MsiQueryFeatureState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ceb4e6d4ef0e7ae7950783254c438595df967e1a) |
| Evan Stade | 2007-07-03 | [gdiplus: Call EndPath() in GdipDrawLineI in case there is an open path.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c60c030c95b17e089fd9b1302c5391fbf708413c) |
| James Hawkins | 2007-07-03 | [msi: Add the IWineMsiRemoteCustomAction interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc4750ff75f83498693cf420d513112c16617420) |
| James Hawkins | 2007-07-03 | [msi: Only publish the product if at least one feature is to be installed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a2df31aea1746fcf067c77af56453100077a336f) |
| James Hawkins | 2007-07-03 | [msi: Return INSTALLSTATE\_ADVERTISED if the component list is empty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=73e0a87477c4b0fe792988061397a5241b72a985) |
| James Hawkins | 2007-07-03 | [msi: Unpublish the product when it is entirely removed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=624bbbe78a68598003eb906ddc1839a250bed340) |
| James Hawkins | 2007-07-03 | [msi: Delay publishing of the SourceList until the PublishProduct action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e46fc9019dce5befe72b50695b8d309aba4f65f) |
| James Hawkins | 2007-07-03 | [msi: Add tests to show when the SourceList is published to the registry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=56129f252c6180be1f75c4698b6bb759344d4490) |
| James Hawkins | 2007-07-03 | [msi: Handle remote calls to MsiGetProperty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4de8247c5a8b914483f589455fa89d9c9313eaa1) |
| James Hawkins | 2007-07-03 | [msi: Handle remote calls to MsiSetProperty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4d668e06a26cdd68fad87e35d0d11008e5efe859) |
| James Hawkins | 2007-07-03 | [msi: Read the components state directly from the registry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39a5638268095be901f4a0103c2be51959cd86ca) |
| James Hawkins | 2007-07-03 | [msi: Return INSTALLSTATE\_BADCONFIG if we can't decode the first component.](http://source.winehq.org/git/wine.git?a=commitdiff;h=34f6af95b4cafc25f06a1ca85c6eb555c34966b5) |
| James Hawkins | 2007-07-03 | [msi: Open the correct key and return INSTALLSTATE\_ADVERTISED if it's missing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1130d5909b102581fb669c7ed3339e657e85cb5f) |
| James Hawkins | 2007-07-03 | [msi: Set the WindowsInstaller value in RegisterProduct instead of PublishProduct.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e44e090c591f485776c7e3898dec5a9e7296f85) |
| James Hawkins | 2007-07-03 | [msi: pcchValue represents the length of szValue in TCHARS, not bytes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cd708e7f5eb91d6ec8c7448180451cf400f062e) |
| James Hawkins | 2007-07-03 | [msi: PackagePath must also include the package name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08443b3bf7f5535dc438b64e9f8aeb9976b64424) |
| James Hawkins | 2007-07-03 | [msi: Add support for the MSICODE\_PATCH option.](http://source.winehq.org/git/wine.git?a=commitdiff;h=04c67c2a1cce0986a2587b9605092b9eef317a4e) |
| Evan Stade | 2007-07-02 | [gdiplus: Use SaveDC, RestoreDC in GdipDrawLineI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d9ef172e04397ffe4a14ba2c87a210e3ad87f45a) |
| Juan Lang | 2007-06-29 | [crypt32: Implement getting content for data messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f75b86f02be0d3caa030b6c89dc66e6338d5717c) |
| Juan Lang | 2007-06-29 | [crypt32: Accept OSS errors as well.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f575d8569bb73dc843ab30daa7c7b305bb813159) |
| Juan Lang | 2007-06-29 | [crypt32: Accept ERROR\_INVALID\_PARAMETER in addition to ERROR\_PATH\_NOT\_FOUND (and ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef134dc70335a76b38d62d52e94c23bd55d2932e) |
| Juan Lang | 2007-06-29 | [crypt32: Accept OSS errors.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e64e66c41d0fd9d0c390308db1554a75f6d69bd0) |
| Juan Lang | 2007-06-29 | [crypt32: Add tests for data message encoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1f379340a5d9936c76db78778fc4ba36e6472a4) |
| James Hawkins | 2007-06-29 | [msi: Return ERROR\_SUCCESS if the PackageName property is not present.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c26505b7016fa593c46a1e9666ba97ceee7f9cef) |
| Juan Lang | 2007-06-29 | [crypt32: Don't fail when CryptVerifyCertificateSignatureEx is missing, use skip (and ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=85eeccc5857df12dbbce4e78b9c7b5beb6c67184) |
| Juan Lang | 2007-06-29 | [crypt32: Implement CryptMsgUpdate for data messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74bf713be79c40be97c37f2a83257e04447300e7) |
| James Hawkins | 2007-06-29 | [msi: Implement MsiSourceListGetInfoA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6cc2f0f4025fcae3fb58ae816bef4c68d8ac48a1) |
| Juan Lang | 2007-06-29 | [crypt32: Use skip to avoid failures where support is missing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68b052057b28f86314538478d0f9834800faaf41) |
| James Hawkins | 2007-06-29 | [msi: Validate MsiSourceListGetInfo parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3e56d78f2eb38b186abaac482c009cef8c4222e6) |
| James Hawkins | 2007-06-29 | [msi: Return ERROR\_BAD\_CONFIGURATION if the SourceList key does not exist.](http://source.winehq.org/git/wine.git?a=commitdiff;h=381b915b475f12e6ecd5fb14bb8fda05c52f2dac) |
| Juan Lang | 2007-06-29 | [crypt32: Implement getting bare content for data messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=263f424c3b27a99553d7d564b9032db17018dd2e) |
| James Hawkins | 2007-06-29 | [msi: Add tests for MsiSourceListGetInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ff40d15587a9c41d2e22a1ae2abb540635a026a) |
| Juan Lang | 2007-06-29 | [crypt32: Accept ERROR\_BADKEY in addition to ERROR\_INVALID\_HANDLE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11e6717e667db19fb5b2ffd4315fba76832809e1) |
| Juan Lang | 2007-06-29 | [crypt32: Add a stub get param function for data messages and remove stub message ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=0546cf1a696125b82843959a5d0d7de36a5abb40) |
| Juan Lang | 2007-06-28 | [crypt32: Stub CryptMsgOpenToEncode for data messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa0f5bd066b6514a14e877fad9dd7836ef5f4ae0) |
| Juan Lang | 2007-06-28 | [crypt32: Test CryptMsgGetParam for data messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e829833986de44ee1ab950594589243dce6815c0) |
| Juan Lang | 2007-06-28 | [crypt32: Add a get param function, use it to implement CryptMsgGetParam.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5e784bdaf7641eafd3bed773f708f39a1eea8e0) |
| Juan Lang | 2007-06-28 | [wincrypt: Add missing message flags and parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c56177a8e945f76d15a67d7b55b23eb2275d1a98) |
| Juan Lang | 2007-06-28 | [crypt32: Test CryptMsgUpdate for data messages opened to encode.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd05e2abe33d042675b56a3d066a3762463e15ca) |
| James Hawkins | 2007-06-28 | [msi: Ignore invalid conditional expressions when checking the launch conditions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bafc4dc3854f59ec0e07aaa202a260c3cf56c5eb) |
| Juan Lang | 2007-06-28 | [crypt32: Add base message type and use it to implement CryptMsgDuplicate and CryptMsg ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b790a09efbd02369b2e3bf0db8a946a15e0a502c) |
| Juan Lang | 2007-06-28 | [crypt32: Add a finalized member to message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6bf594aa571731392acace33cab4ae731a4dbc5) |
| Juan Lang | 2007-06-28 | [crypt32: Test CryptMsgOpenToEncode for data messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a581855d263ad259ba63e19856a55a8b0cd420a0) |
| Juan Lang | 2007-06-28 | [crypt32: Don't return fake HCRYPTMSG from CryptMsgOpenTo\*.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6c054f057b75cf0257d78d50f70db5eafb5fc658) |
| Juan Lang | 2007-06-28 | [crypt32: Add an update function, use it to implement CryptMsgUpdate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5db6b1cc962d0ab8c3bb6e9f05ef534437c91af3) |
| Juan Lang | 2007-06-28 | [crypt32: Add basic tests for CryptMsg functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3de0e4ac48bedb67c0402ad8ad1de38521eecc83) |
| James Hawkins | 2007-06-28 | [msi: Add tests that show '!=' is not a valid conditional expression operator.](http://source.winehq.org/git/wine.git?a=commitdiff;h=219857f831616811aa36275d1c6c0098b4ce6a2f) |
| Juan Lang | 2007-06-28 | [crypt32: Store stream info in message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=203849d75d0a62e1b1b970cb73941755642f8123) |
| Juan Lang | 2007-06-28 | [crypt32: Add basic parameter checking to CryptMsgOpenTo\*.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1c837f16ace9217bcad618149c85d6932542fde6) |
| James Hawkins | 2007-06-27 | [msi: Set the WindowsInstaller value of the UserData product key when publishing the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=c18b77557d60017ef3f3c2eea5782bae17126006) |
| James Hawkins | 2007-06-27 | [msi: Use the correct registry key when detecting a published product.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7da89f48fd44c54e8b963e94b5f69d88b6334c57) |
| James Hawkins | 2007-06-27 | [msi: Add support for remote handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=46158e034cb0f17f32d5c7516df96f1a5ded6093) |
| James Hawkins | 2007-06-27 | [msi: Any value of WindowsInstaller besides 0 means the product is installed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3bf32f27005a0e529d0ef614d407a85fee8f5238) |
| Evan Stade | 2007-06-27 | [gdi32: Added missing call to GDI\_ReleaseObj.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39357c4ba6a862bbe257b6ac9691ee40564e9b81) |
| James Hawkins | 2007-06-27 | [msi: If the UserData product key exists, but the user product key doesn't, the produc ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=24ede2f9e602b24080f47134055f9a1e540f487c) |
| Dan Hipschman | 2007-06-26 | [widl: Check for interface pointers in pointer handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcebe48cadcc1abfca71f1a78bba06bd0c858fca) |
| Lei Zhang | 2007-06-26 | [comctl32: Reduce duplicate code between PROPSHEET\_CollectSheetInfoA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4dd14abc6ddf7b1b1f50bf75df8b857af85f6aa) |
| Dan Hipschman | 2007-06-26 | [rpcrt4: Allow enums as union switch types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea7b1694de36742f0b3b356a6bebf5d181619583) |
| James Hawkins | 2007-06-26 | [msi: Validate MsiQueryProductCode parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e92f66558a8f415cee051d8752438726dbd64bc1) |
| Lei Zhang | 2007-06-26 | [comctl32: Determine if PSH\_PROPSHEETPAGE is set once.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e3b80a0d882239a7bebb03ac49ee4698c1e9be43) |
| James Hawkins | 2007-06-26 | [msi: Add tests for MsiQueryProductState.](http://source.winehq.org/git/wine.git?a=commitdiff;h=db318ec9afd96b49950dc8f06dcfe6586f135263) |
| Dan Hipschman | 2007-06-26 | [widl: Check for user types when calculating buffer size.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ab22b4b3d45717831c4f5ce82de2e0705d0735d4) |
| James Hawkins | 2007-06-26 | [msi: Add tests for publishing and unpublishing products, features, and components.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90e9722ecb03529deab340d22018cdfdbea560c7) |
| Dan Hipschman | 2007-06-26 | [widl: Fix crash dealing with anonymous unions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=704f2868ed0c1350a08a2991b7db4cf086ef3389) |
| Dan Hipschman | 2007-06-26 | [widl: Get simple enums working.](http://source.winehq.org/git/wine.git?a=commitdiff;h=512c36cae62fa0d45ac1997abf4eb0149ce264cd) |
| Dan Hipschman | 2007-06-26 | [widl: Allow enums as union switch types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=46222aee6ea7577ba060d1907d29ca5a8651a524) |
| James Hawkins | 2007-06-26 | [msi: If the user product key exists, the product's state is advertised.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15823e1acfab45d975a0239efd9fafa7e8dd741e) |
| Lei Zhang | 2007-06-26 | [comctl32: Reduce duplicate code between PropertySheetA/W.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cbee494b34354b533346eece60e03f6cdaf9cab) |
| Dan Hipschman | 2007-06-26 | [rpcrt4/tests: Wrap a try/except block around tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=076a6206ff9598af97e940b62b8b629da4758e6d) |
| James Hawkins | 2007-06-25 | [msi: Add a stub implementation of MsiQueryComponentStateA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee89cfca534679d72b23a79165b6a74e5fc19b40) |
| James Hawkins | 2007-06-25 | [msi: Fetch the volume name when getting disk info.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71d7da11707b5ccdb7aec9664c01aaa56c9e349f) |
| James Hawkins | 2007-06-25 | [msi: Reference count the custom action data to avoid freeing the data by another ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=4c3e4ba02907f780d7bb78acc646115b5792765d) |
| Evan Stade | 2007-06-23 | [gdiplus: Fix broken graphics path constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6baacf61a857a7f9c471005cb12553f8d37a558e) |
| Evan Stade | 2007-06-23 | [gdiplus: Tidy up graphics constructor.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6490dadb2396b8b495e681b6bbfd2a22acac355b) |
| Evan Stade | 2007-06-23 | [gdiplus: Fix erroneous pen error checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=02efd4bbf1afdc9cba8c7e824d85bb7f7b6a7319) |
| Evan Stade | 2007-06-21 | [gdiplus: Implemented GdipDrawLines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f6f04f6e0ede8f7add6db6874a2c294fc993e900) |
| Lei Zhang | 2007-06-21 | [winex11.drv: Reset focus if application does not want to be activated.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e20625e5c95a1852c6ce9e38334f2a187114d602) |
| Nigel Liang | 2007-06-21 | [winex11.drv: Remove call to XCreateFontSet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f3a02ea2fd66514c59edd7ed95bb2e0df581350) |
| Evan Stade | 2007-06-21 | [gdiplus: Implemented GdipCreatePath and GdipDeletePath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14802872b876581fc895f5310e120f83b88b58dd) |
| Dmitry Timoshkov | 2007-06-21 | [shell32: Make SHGetDesktopFolder use a cached instance of IShellFolder.](http://source.winehq.org/git/wine.git?a=commitdiff;h=013652feeef3a69d43cedb7ad431010f1e4dbcdc) |
| Evan Stade | 2007-06-20 | [gdiplus: Implemented GdipDrawArc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c42f8794a1519ac0dba46c7c638372ba3310b121) |
| Dan Hipschman | 2007-06-20 | [widl: Fix warnings about unused function parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf5e46a60aa1cfcbb6efd61ebf4d34eb9fb0084d) |
| Evan Stade | 2007-06-20 | [gdiplus: Implemented GdipDrawCurve2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c8b83c524c7059edc4b9ef14f88c08f9760506e) |
| Dan Hipschman | 2007-06-20 | [widl: Add tests for arrays of pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e8c8d03e50a13c62711a3afb1bb424a56a9382a) |
| Dan Hipschman | 2007-06-19 | [rpcrt4: Fix typo in union buffer size calculation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d2c15ed01bd0a0766b0b4f6e364a1ad58b333141) |
| Dan Hipschman | 2007-06-19 | [rpcrt4: Remove inaccurate comments.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b09b917a5c2c3f7f615d224500501318b994150b) |
| Evan Stade | 2007-06-19 | [oleaut32: Save load time format of pictures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72e20d8f57980586dc3745b6fd53e47c84d4faca) |
| Dan Hipschman | 2007-06-19 | [rpcrt4: Fix bug calculating union switch type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6fd05b1dc7c83743bae5fb1e04941ec3bd560490) |
| Evan Stade | 2007-06-19 | [oleaut32: Added support for decoding some PNG files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5c5c5aabc549044e1c200e5932b7c5bd835e84be) |
| Dan Hipschman | 2007-06-19 | [rpcrt4: Add encapsulated union tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08c846a9da942656f2f463154e141e91f03f1112) |
| James Hawkins | 2007-06-18 | [ntoskrnl.exe: Add a stub implementation of KeInitializeTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fbbd91544f2ad1cb179ee6f3cbe124f8a9b79f18) |
| Lei Zhang | 2007-06-18 | [winex11.drv: Send WM\_MOUSEACTIVATE before closing a window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a67bded8c5b6ba48470f30437564b3ae1437ef6) |
| James Hawkins | 2007-06-18 | [msi: Properly delete rows from the table, instead of zeroing out the row.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9309f4dfa0f82e3ed2d3582a33fad5eb6a321498) |
| James Hawkins | 2007-06-18 | [msi: Send the expected data to set\_deferred\_action\_props.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82f4e3981bacb58625f1d72893342b8d328365c5) |
| Evan Stade | 2007-06-18 | [gdiplus: Implemented GdipDrawPie/GdipFillPie.](http://source.winehq.org/git/wine.git?a=commitdiff;h=72ab72c50c370372b214bb72814109637db88733) |
| Lei Zhang | 2007-06-18 | [riched20: Add tests for EM\_FORMATRANGE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=55771014e12310ab9c98f9e1bb9e6f0a455fb090) |
| Evan Stade | 2007-06-16 | [gdiplus: Implemented GdipDrawBezier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b9f5342b4ba291ab311f7c2b5a4d554083ab900) |
| Lei Zhang | 2007-06-15 | [comctl32: Make modal property sheets modal.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ebb460c3c0c227392699fd1b0809f6f35ea52847) |
| Dan Hipschman | 2007-06-15 | [widl: Handle encapsulated unions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4679b0c139c83a8e3ceff8033d4442b6f772c3b) |
| Dan Hipschman | 2007-06-15 | [widl: Factor the output functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e36981e1168e2f4639fd71202a65252dfb1b555e) |
| James Hawkins | 2007-06-15 | [msi: Implement MsiApplyPatchW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d8860d34e4008299320a0cbd0aea033b608a1395) |
| James Hawkins | 2007-06-15 | [msi: Forward MsiApplyPatchA to MsiApplyPatchW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=974e76fe79b54ba98196e637d6d4372f56e50aea) |
| Dan Hipschman | 2007-06-15 | [widl: Handle embedded interface pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8709a06028709b11ade91087c1bdba8678adc65c) |
| Dan Hipschman | 2007-06-15 | [widl: Fix a write\_parameters\_init bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=58dea5c9a833b6587944d36f02a59ff4794fed29) |
| James Hawkins | 2007-06-15 | [msi: Patches are applied based on ProductCode, not ProductID.](http://source.winehq.org/git/wine.git?a=commitdiff;h=261e1179bb2903590794473668dc93ffd3785ff7) |
| Lei Zhang | 2007-06-14 | [comdlg32: Move file dialog resizing code into its own function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eef9e1ab882fe1f74f84c23b1d4a68b34b65d7fe) |
| Evan Stade | 2007-06-14 | [gdiplus: Brush tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4fdc9690c6b12e0dc0db4f064100724e378a75e) |
| Lei Zhang | 2007-06-14 | [user32: Remove a unused variable from ES\_PASSWORD test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dd88237d3ec21ec44bdd500bad02b079c9894943) |
| Evan Stade | 2007-06-14 | [gdiplus: Brush implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cc0a676b22134a68b69f8f268ca308c3920bc0f2) |
| James Hawkins | 2007-06-14 | [msi: Fixed the WriteEnvironmentStrings action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=881f59254a1d2e1fc0b8661c3f0f14d709e80007) |
| Lei Zhang | 2007-06-14 | [user32: Improve cut/copy/paste behavior of password edit boxes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7dd98bb993b886922b07954a3956f32763ea58c1) |
| James Hawkins | 2007-06-14 | [msi: Set the UserSID and ProductCode properties for deferred custom actions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c444ea350e0688247bd2056b3861dac4af08fbc) |
| Dan Hipschman | 2007-06-13 | [widl: Handle wire\_marshal types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c0982b42c5293f22b0be0cc3d06e8a2a7ef0e9f9) |
| James Hawkins | 2007-06-13 | [msi: Protect custom actions with a structured exception handler.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9ed5c865e219d4d55ab1da32ccb8f7922343c092) |
| Dan Hipschman | 2007-06-13 | [widl: Handle wire\_marshal pointer attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=33250206364dc66451a07abb72f658b84d729ed4) |
| Dan Hipschman | 2007-06-13 | [widl: Test structure argument marshalling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2bc8808be1f2b4599412321f58311f176101d09b) |
| James Hawkins | 2007-06-12 | [msi: Set the MsiNetAssemblySupport property.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8a8f77abe87945c48330482c1d94a3d0c527edb) |
| Dan Hipschman | 2007-06-12 | [widl: Simplify correlation descriptor code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=88c812870430b7031c620d91c974dd5e64e8b687) |
| Evan Stade | 2007-06-12 | [gdiplus: Implemented GdipDrawRectangleI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b9bfbe7b726981549609fc9d8e7071236b5696a) |
| Evan Stade | 2007-06-12 | [gdiplus: Implemented GdipDrawLineI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2689b18ea4fcbb3adb65919960aca7b78ab42a8b) |
| Evan Stade | 2007-06-11 | [gdiplus: First pen test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcd7a62e930f9ed55cbb31a18efd011845c646bc) |
| Evan Stade | 2007-06-11 | [gdiplus: Added first GDI+ graphics implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d50be49775ce850e9f045e9c4272d3e8137e3159) |
| Evan Stade | 2007-06-11 | [gdiplus: First pen implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63bfd40f6177ca6bd54ac5497f84377e914e818b) |
| Dan Hipschman | 2007-06-08 | [widl: Check for NULL in set\_tfswrite.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b186c4dd0e7bcb92f147fc00e473e495deaef62b) |
| Evan Stade | 2007-06-08 | [gdiplus: Added beginnings of memory and startup functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a781bbf096d9a3264fe52fa90891b5a19fca9e4d) |
| Dan Hipschman | 2007-06-08 | [widl: Fix incomplete struct/union typedef bug.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e22899e1316e86e2fc812d2540c7aff04925044) |
| Evan Stade | 2007-06-08 | [gdiplus: Added public headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=48f10d4bbff73e2d246b3b5c1f7e4d73a40f28ed) |
| Nigel Liang | 2007-06-08 | [shell32: Conformance tests for unicode filenames and fix a bug for file deletion.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1fc0cb75eebeb011a1f620fb96f32245d886916c) |
| James Hawkins | 2007-06-07 | [msi: Add support for large string tables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a05613a9f29914b0df425d2592f35efd8343b517) |
| James Hawkins | 2007-06-07 | [msi: Represent table data as bytes instead of shorts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8568e0a4a8f9d6b7cc391fa0041b61389c2d1f45) |
| Lei Zhang | 2007-06-07 | [shell32: Start implementing BIF\_USENEWUI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7318ae2411eea8e43aa931bbbe676dc2fb7fa233) |
| James Hawkins | 2007-06-07 | [msi: Reduce the amount of code that directly accesses table data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=65f23343ee86fea1f7001684658bf12be1c5a43f) |
| James Hawkins | 2007-06-07 | [msi: Use fetch\_int to reduce code duplication and access to table data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=298699e2426e2e2687d5d655e73ccd9ecd3db2fc) |
| Dan Hipschman | 2007-06-06 | [widl: Replace get\_name with a field reference.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5baddf88a4061507f470c45c90b2fc374bd5175) |
| Dan Hipschman | 2007-06-06 | [widl: Represent arrays with type\_t.](http://source.winehq.org/git/wine.git?a=commitdiff;h=978b4d4f4e7acb119b1acd59091bfb96bdfd1dd4) |
| Dan Hipschman | 2007-06-06 | [widl: Implement conformant structure handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f689ee023220264790802b625238ce7525b445a) |
| Dan Hipschman | 2007-06-06 | [list.h: Add macros for reverse iteration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6cf8e6bd77f6d3c98f39740ce9c789762a7eb52c) |
| Lei Zhang | 2007-06-05 | [wined3d: Various spelling fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f00670df6135eba1cb162aac954765619ce5f605) |
| James Hawkins | 2007-06-01 | [msi: Implement SummaryInfo::Property get.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f083b3c038eb5b849bfd838a78f32a5f59f0774c) |
| James Hawkins | 2007-06-01 | [msi: Implement Installer::OpenDatabase.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a289624cfcbc829aabc614093bbd5ae01251529) |
| Dan Hipschman | 2007-05-31 | [rpcrt4: Fix build of test on Solaris by renaming a variable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e5c8a6eb5d5e278f5997d7082f2f4223fc1d6807) |
| James Hawkins | 2007-05-31 | [msi: Add handling for MsiBreak.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60e95ee6e8ea4a4f43a6c170c917fc7285b76455) |
| James Hawkins | 2007-05-30 | [wintrust: Add stub implementations for CryptCATAdminAddCatalog and CryptCATAdminRelea ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=98350044d5c184445430700c0f916142b693883c) |
| James Hawkins | 2007-05-30 | [msi: Implement the WriteEnvironmentStrings standard action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b8641a5a43d53f225d6e4c6b1d4ceda90183f3e) |
| James Hawkins | 2007-05-29 | [msi: Perform a forced reboot if a custom action returns ERROR\_INSTALL\_SUSPEND.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2e91588e9bb470e109e3990799df451b47b0cd6) |
| James Hawkins | 2007-05-29 | [msi: Set the MsiNTProductType property.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8e0b3c1c82a494baddaeceb55844082eab21ed9) |
| James Hawkins | 2007-05-29 | [msi: Fall back to checking if the cab exists if the volume name doesn't match.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44649d2ff869394c1fa3ef89fdc43395b2214fc7) |
| James Hawkins | 2007-05-29 | [msi: Create the destination directory if it doesn't exist when duplicating files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1aa0082558050daed4852ad29cc0a12c531a35e6) |
| Evan Stade | 2007-05-25 | [gdiplus: Added stub implementation of gdiplus.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bed761c9e72febb3b2d681fd4e540e149af9e71a) |
| Dan Hipschman | 2007-05-25 | [rpcrt4: Fix test typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b4e8073f8cceb1a5a1376253e24e6e6347ee16ad) |
| Dan Hipschman | 2007-05-25 | [widl: Shrink type\_t structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c30da77ba074d18f2d52891c9bbb32ede6e96a2) |
| Dan Hipschman | 2007-05-25 | [widl: Allow types that reference themselves.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f7a5d63ec8a96d24c8f56eca7f49b390e1de9af) |
| Dan Hipschman | 2007-05-25 | [widl: Handle pointers in unions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00ce411231b4dd94fef20e98b1a9c08c3321670e) |
| James Hawkins | 2007-05-24 | [msxml3: Add initial implementation of IXMLDocument.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5e9a1ea6f6eb7e750ff09060937ea91012b8985) |
| James Hawkins | 2007-05-24 | [msi: Remove a misleading ERR, as this fails if a file doesn't exist, which is common.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5c2806ca19bfcfe1c7d3002714b4df829a9d650) |
| James Hawkins | 2007-05-24 | [msi: Add the ability to deformat the component's source.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea2c96c5dfb42a5efceeaf6d044953b93a2de5f3) |
| James Hawkins | 2007-05-24 | [msxml3: Add tests for IXMLDocument.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e24667cc6e5f5dd1e3434d9073496970130de4e0) |
| James Hawkins | 2007-05-24 | [msxml3: Add tests for IXMLElement and IXMLElementCollection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c04d0d8ca8811f5ddfc66c987c83a50075a1da9) |
| James Hawkins | 2007-05-24 | [msxml3: Add initial implementation of IXMLElement and IXMLElementCollection.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74f18d968ffb75a307932879810ecf87b4c9f915) |
| Nigel Liang | 2007-05-22 | [shlwapi: Stub implementation for SHSetTimerQueueTimer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ddbb317915f7cfb1dd6f48431f4fde43527eb068) |
| Lei Zhang | 2007-05-22 | [include: Add missing definitions to shlobj.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00bc8fa184f2df997ffab28e307b9ddbd6e94181) |
| Dan Hipschman | 2007-05-18 | [widl: Lay framework for unions with simple unions working.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c5aaadc4c89a49696dc265cb1498e2e28837534a) |
| Dan Hipschman | 2007-05-18 | [widl: Replace erroneously removed current\_func assignment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=18724eaeb8534a04f9d530692f2bee42cb87f58b) |
| Dan Hipschman | 2007-05-16 | [widl: Write some structures to the type format string on the fly.](http://source.winehq.org/git/wine.git?a=commitdiff;h=52ca3ebadac7eb1132fce34e750d4d96b48e052c) |
| Dan Hipschman | 2007-05-16 | [widl: Improve handling of offsets in the type format string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=217fc9c0f3d5d514eb0a2cf352783374855ce17c) |
| Dan Hipschman | 2007-05-12 | [widl: Remove an unnecessary assignment in write\_pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=faf50715493df83b38e43176cb2d13c4149a0ed9) |
| Dan Hipschman | 2007-05-12 | [widl: Handle pointers fields that point to structures.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d9c120490fbea62f5696ed99c7f4d8390f9dfef4) |
| Jacek Caban | 2007-05-11 | [mshtml: Split code from OnDataAvailable.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98da8e2823f4ab5aff8bb25a5fe80995fcd8e935) |
| Jacek Caban | 2007-05-11 | [mshtml: Don't crash in OnStopBinding if This-&gt;binding is null.](http://source.winehq.org/git/wine.git?a=commitdiff;h=94a264d0beef21f51655e3cacebc699e74ee4d7b) |
| Jacek Caban | 2007-05-11 | [mshtml: Added IPersistStreamInit::Load implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=920f628c6e6934131608db98388ad4f06ac8b862) |
| Jacek Caban | 2007-05-11 | [mshtml: Added IPersistStreamInit::Load test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=66067781d6e5df7499abe419216172e630383056) |
| Jacek Caban | 2007-05-11 | [mshtml: Move AddRequest call to the separated function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2dd9fad610ea4197c3b71352c9cdaa5db4d8daac) |
| Jacek Caban | 2007-05-11 | [mshtml: Split IPersistMoniker::Load.](http://source.winehq.org/git/wine.git?a=commitdiff;h=09adb8cf051ac76df81260afd68a99974c2bbd6c) |
| Dan Hipschman | 2007-05-10 | [widl: Remove var\_t's ptr\_level field and start write\_pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ef433e279295beeadcbec3f36016ffc3587834a3) |
| Dan Hipschman | 2007-05-10 | [widl: Remove redundant get\_var\_vt function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e7495555a09e1c5631d7de77926a95bf3f551201) |
| Dan Hipschman | 2007-05-10 | [widl: Add string\_of\_type function, prettify code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=933ca7b126c12c222a7c5509c266f96af8221b9a) |
| James Hawkins | 2007-05-10 | [msi: Only check the volume label for every media after the first disk.](http://source.winehq.org/git/wine.git?a=commitdiff;h=666cfd1c0346904dc5d3c27eee80ce871bec26ca) |
| Dan Hipschman | 2007-05-10 | [widl: Simplify make\_safearray.](http://source.winehq.org/git/wine.git?a=commitdiff;h=541dddfde37120d1334dade507e390836403bf82) |
| Dan Hipschman | 2007-05-10 | [widl: Remove dead code in write\_msft.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=234855f059a374c76783c180dd00193023da6aff) |
| James Hawkins | 2007-05-10 | [msi: Deformat the key path before opening the key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0de574b258b86c1399af5a53485280e4eb8b7952) |
| James Hawkins | 2007-05-09 | [msi: Check the volume name when changing media.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6eb7eadffa5e9863722058325c0977142cd9af49) |
| James Hawkins | 2007-05-09 | [msiexec: /quiet is the same options as /qn.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b8bad751894a523d75865d4bc2be7264cd2c924) |
| James Hawkins | 2007-05-07 | [msi: Remove debugging printf statements.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e962b0a7df3bc4405d1c94b0b0054f4e6cdb60e3) |
| James Hawkins | 2007-05-07 | [msi: Add stub handlers for the remaing standard actions that reference tables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=987c2c85e136f077e52390acf04ef09fdb80cade) |
| James Hawkins | 2007-05-07 | [msi: Set the text limit of the edit control if the limit is given.](http://source.winehq.org/git/wine.git?a=commitdiff;h=933fd8b8797b340558e06b5d19e51d94b068c5ab) |
| James Hawkins | 2007-05-07 | [msi: Add the ES\_AUTOHSCROLL style to the edit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7fe3ba934cb0f4908d20a9136b36f206c1b78fa6) |
| James Hawkins | 2007-05-07 | [msi: Only allow valid styles in msi\_dialog\_get\_style.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f4a4e161f561a8e7416e918c4e57affee688193) |
| James Hawkins | 2007-05-07 | [msi: Add handling for the ReinstallMode control event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=770e49cd3c67851c3c6fc0222cd220d6b2e21015) |
| James Hawkins | 2007-05-07 | [msi: Remove incorrect ERR as messages can be sent before the control is created.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12c33ab8aa0d314c21afbfc850f94201faa58cf9) |
| James Hawkins | 2007-05-01 | [msi: Add tests that show that costing is run in both the UI and Execute sequences.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d8586e164f7892c480db3a1427b4ec6a6be98c05) |
| Dan Hipschman | 2007-05-01 | [widl: Get rid of the tname field of var\_t, simplify code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d676d3be5fce72d35cb9eb7063ace424f3bcf78e) |
| James Hawkins | 2007-05-01 | [msi: Reset the folder's resolved target before setting the target in CostFinalize.](http://source.winehq.org/git/wine.git?a=commitdiff;h=baad888766850ad390079a3abdf561517b61ef33) |
| Dan Hipschman | 2007-05-01 | [widl: Get rid of the typeref\_t structure, simplify code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ecbb01617909b0ed149448afc5c8c81e75acb3b) |
| James Hawkins | 2007-05-01 | [msi: Run the costing actions for both the UI and execute sequences.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1104dc088df7f0f492c1bc6b48258d8a2ce9a956) |
| Dan Kegel | 2007-04-28 | [advapi: Improve SetEntriesInAclA stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=67e2c97a88ce75dbbe22eefcd3137bf8315786e2) |
| Dan Hipschman | 2007-04-26 | [rpcrt4: Add a testcase for RPCs with fixed-size arrays.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba17c25e62970340a67d0e15d818694d87143fcb) |
| James Hawkins | 2007-04-25 | [msi: Implement special handling for the \_Streams table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da55285acba1839fca9cf93422a42eac062760ed) |
| Lei Zhang | 2007-04-23 | [comdlg32: Initialize CommDlgExtendedError() return value for file dialogs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7aa1b2e419976a14495227bfd45b37cdae219207) |
| James Hawkins | 2007-04-21 | [msi: Return MSICONDITION\_NONE in MsiDatabaseIsTablePersistent if the table doesn't ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d677bd7f3b43cd94fcf95bfed035b4e817fffd34) |
| James Hawkins | 2007-04-21 | [msi: Add the \_Property table back, with tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b4bb6e5b5d5b85f0bc4bbbad2b6a8ec3872a5759) |
| James Hawkins | 2007-04-21 | [msi: Abstract MSI\_RecordSetStream.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7d3162e6bed476c937a8d2f3d1b44c8076959e61) |
| James Hawkins | 2007-04-21 | [msi: Add an internal MSI\_ViewModify.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b4bf44b793fa1dcf102289b2c789a3284669f07) |
| Lei Zhang | 2007-04-20 | [wineshelllink: Fall back to $HOME if $HOME/Desktop does not exist.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d0c83654f8a9928be13539714c723d2ec9cfe0a5) |
| James Hawkins | 2007-04-15 | [msi: Add handling for the concurrent install custom action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98eafa870c619dbf78ae28feb8f5abc904de5cb9) |
| James Hawkins | 2007-04-15 | [msi: Run the InstallExecute sequence if the InstallUISequnce table is empty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6da8041d4752e86d65d46348f84810bcd99c823a) |
| James Hawkins | 2007-04-15 | [msi: Add tests for the concurrent installation custom action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4cc48b7710eead6051652eb646c44d82f741bcab) |
| James Hawkins | 2007-04-15 | [msi: Generalize the msi\_custom\_action\_info struct so other custom actions can use it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06df9f790d175432be7352ae555bb441c21a351e) |
| Lei Zhang | 2007-04-13 | [comctl32: monthcal: GetMonthRange Tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf7b0b89fedd4ac3b9adfa143e6f05638cfb6838) |
| Lei Zhang | 2007-04-12 | [user32: WM\_ACTIVATEAPP on minimize message test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c569ab2a6727ce7cef6ca6e90f398c50640493bc) |
| Dan Kegel | 2007-04-12 | [winex11.drv: GetAsyncKeyState must check mouse buttons, too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c2ae970e6055f6d18a9166c4cd2d760edfabf20d) |
| Lei Zhang | 2007-04-12 | [comctl32: More monthcal hit tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b47a756ac7d7d1b158c2f37006c7e60fc1db37ab) |
| James Hawkins | 2007-04-11 | [msi: Reset the is\_extracted flag when every cabinet is loaded.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7ef8428b5e5e14c5a048d7a655b68249178837c1) |
| Lei Zhang | 2007-04-10 | [comctl32: Fix first day of the week in monthcal.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6fb16fca6beeaf80c1c0294ebeff88da13e28950) |
| Lei Zhang | 2007-04-06 | [advapi32: Spelling fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d347ebe1968a32d62834d897ecfed647e001c06a) |
| Dan Kegel | 2007-03-31 | [imagehlp: BindImageEx stub should report success.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71971409c8489b1c52dda8ac3a2d46788a18d9b9) |
| James Hawkins | 2007-03-29 | [msi: Load the folder property if available and requested.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8cedb218c314f444612fd3dea67a8834d2f596e9) |
| James Hawkins | 2007-03-28 | [setupapi: The Inf file should be copied regardless of the destination buffer, with ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff326fd0ffd4ad017634d6d068781d8a0736d4a2) |
| James Hawkins | 2007-03-28 | [setupapi: Don't allow relative paths in SetupCopyOEMInf.](http://source.winehq.org/git/wine.git?a=commitdiff;h=efa6591fff772c7fc88f3dd26500610f55d6b551) |
| James Hawkins | 2007-03-28 | [setupapi: Correct the Inf output position.](http://source.winehq.org/git/wine.git?a=commitdiff;h=672952d2b6abf525d3ccd73b68ee418f51f8eae2) |
| James Hawkins | 2007-03-28 | [setupapi: SetLastError to ERROR\_SUCCESS on success.](http://source.winehq.org/git/wine.git?a=commitdiff;h=405b96e979dcb751988e061cd1f78319232d3d84) |
| James Hawkins | 2007-03-28 | [setupapi: Handle the SP\_COPY\_NOOVERWRITE flag.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3e5f62b2d8d7353f890ca6e4fb27809c9f7dae8f) |
| Jacek Caban | 2007-03-28 | [mshtml: Added DispHTMLDocument dispinterface declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=394c3f9adbc9952e1deb3932cab36cc1e0f63f0e) |
| Jacek Caban | 2007-03-28 | [mshtml: Added DIID\_DispHTMLDocument to QueryInterface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b94f19cb93dd2728b81a055f4a168edd96eaf9a) |
| Jacek Caban | 2007-03-28 | [winnt.h: Added activation context structures declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06bd1bf8e1620da270a90e1c7640634397506704) |
| James Hawkins | 2007-03-26 | [setupapi: Add missing SetupCopyOEMInf flags.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da85c0905d26ddc31a8deb7b426b41e75fac2b44) |
| James Hawkins | 2007-03-26 | [setupapi: Add several tests for SetupCopyOEMInf, with fixes so the tests don't crash.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9eaea34e041671fa63095a825c32978d1a9780d5) |
| Jacek Caban | 2007-03-19 | [spoolsv: Added spoolsv.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1ddc9c1f72e796fba3997c07dc04a1d822a6e29) |
| Jacek Caban | 2007-03-19 | [spoolss: Added RevertToPrinterSelf stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c88ccdc1ef9c63a416024461a92d6e5bb98db347) |
| Jacek Caban | 2007-03-19 | [wine.inf: Register Spooler service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=546de27f1124b974bd777ec833964ae7731f736d) |
| Jacek Caban | 2007-03-19 | [advapi: Improve SetEntriesInAclW stub.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2cd033eee1a2f442d40a4c1663d500ac7e5ef9c0) |
| Jacek Caban | 2007-03-19 | [advapi: Constify argument of StartServiceCtrlDispatcher[AW](http://source.winehq.org/git/wine.git?a=commitdiff;h=112257e59db7cc8c60a151b190f5cc4c074ed46d) functions.] |
| Dan Kegel | 2007-03-12 | [advapi32: RegGetKeySecurity needs to pass length of struct to caller.](http://source.winehq.org/git/wine.git?a=commitdiff;h=60cb73b573d139f49b4445318ce3762685a9ff87) |
| Lei Zhang | 2007-03-02 | [regedit: Correctly parse key name containing '](http://source.winehq.org/git/wine.git?a=commitdiff;h=4de636208f503cce544cebd2564143635b41c462)' when deleting/exporting.] |
| Lei Zhang | 2007-03-02 | [regedit: Allow entering - for a key in a .reg file to delete that key.](http://source.winehq.org/git/wine.git?a=commitdiff;h=054fd8cb42fb3b3b13fee48a7747f0063d853f09) |
| Lei Zhang | 2007-03-01 | [regedit: Correctly parse key name containing '](http://source.winehq.org/git/wine.git?a=commitdiff;h=d113419682a1a723336dafa53f2d81c223fad395)'.] |
| Lei Zhang | 2007-03-01 | [regedit: Updated English resources to remove shortcut conflicts.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f05d80aa966ad40db6aab37dc26527d8c8cd7fd) |
| Lei Zhang | 2007-03-01 | [regedit: Removed dead code from regproc.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a54a89b8bc4ce4d3cb09bae846f8ac5903f552d) |
| James Hawkins | 2007-02-28 | [comctl32: Add message ids to allow multi-window test sequences.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2b5f79c9a851961024a2dbffbf2160f698baa6b3) |
| James Hawkins | 2007-02-26 | [msi: Overwrite an existing read-only file when copying the install file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba40c463d76235474249b92654d3f9caee5778b7) |
| James Hawkins | 2007-02-25 | [msi: Check for a NULL text entry, as it can be blank in the VolumeCostList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4a324940b3b92595dd26a92561cc80b01b0a3bd) |
| James Hawkins | 2007-02-25 | [msi: Add tests for using markers in SELECT clauses.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a40d687133b962128ed61ef0264dc3e14f861491) |
| James Hawkins | 2007-02-25 | [msi: Free the custom action data after the thread function executes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=747f19f01196cba5a24a1f60a306f815ef4763b0) |
| James Hawkins | 2007-02-20 | [msi: Cleanup the dialog event subscriptions when destroying the dialog.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0746b9076d2c32906de4d291e1ce8f809927988c) |
| Lei Zhang | 2007-02-17 | [comctl32: Move up-down msg seq test functions into msg.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b29c99c59a59d9aff82518a108de61f088cb1b34) |
| Lei Zhang | 2007-02-13 | [tools/wineshelllink: Create links with WINEPREFIX.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a3a144896e2acf6c40e8e90a17b3478622d8450) |
| James Hawkins | 2007-02-08 | [msi: Don't skip files continued from a previous cabinet.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b8282120a676e66a0e767438cb8abfe43bddd58) |
| James Hawkins | 2007-02-04 | [msi: Allow uncompressed files before compressed files in the same media.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30577c253a7095184e00a4881c7d05d8a4cb5636) |
| Dmitry Timoshkov | 2007-01-23 | [user32: Using DIB APIs to convert a DDB to monochrome is wrong, do it differently.](http://source.winehq.org/git/wine.git?a=commitdiff;h=81a294f76d47fcacdfff185617f27c6872d578fd) |
| Dmitry Timoshkov | 2007-01-23 | [user32: Do not use DIB APIs for bitmap bits in a device dependent format.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7670d76690f12a240ec0241a4bd96b8f5f5a7c6a) |
| Dmitry Timoshkov | 2007-01-22 | [gdi32: Add a GetDIBits test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f31b67ae441b87028a236898572efbe359d16b88) |
| Lei Zhang | 2007-01-22 | [comctl32: Fix the updown control test to use the optional flag.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4de56b1b4dc3a741f68f49efd19d157b1084f6c0) |
| Dmitry Timoshkov | 2007-01-22 | [gdi32: Add a simple SelectObject test for bitmaps.](http://source.winehq.org/git/wine.git?a=commitdiff;h=295f8101ec882bd62042ff4526f0cb3f6c2cf5bf) |
| Dmitry Timoshkov | 2007-01-18 | [user32: Some apps pass a color bitmap as a mask to CreateIconIndirect, convert it ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=64f1d97a5435df2f8275c304145635bce290db14) |
| James Hawkins | 2007-01-16 | [oleaut32: Initialize nrofnames to keep from freeing unused memory in the error case.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8eb80763956d5b618d5f5ab30ddabb72d81a736) |
| James Hawkins | 2007-01-16 | [advapi32: Add tests for RegQueryValue.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6cc4510b719a0014afe948c59fb274c362a45b70) |
| James Hawkins | 2007-01-11 | [mshtml: Use the correct variable in the FIXME.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d06ff0ea6909fa2ba12bf296565191e857384fb4) |
| James Hawkins | 2007-01-11 | [winedbg: Check buffer for NULL before writing to it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8be71fef5ba74034170259e40a2ec3cec5ac0942) |
| James Hawkins | 2007-01-11 | [winspool.drv: Check for get\_filename failure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=68406933714001224b367d4d6f40f563c00fd092) |
| James Hawkins | 2007-01-10 | [advpack: Fill the output buffer to workaround a bug in IE7s advpack.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b3331d1a76a5116b391b0757bfcf6752a307d3d3) |
| James Hawkins | 2007-01-10 | [comctl32: Rewrite the up-down control tests to add message checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74ada83c60fd153bbcb45fe41deda326b79f4816) |
| Lei Zhang | 2007-01-03 | [comctl32: Add initial tests for the status bar control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a463f039b544ad27ae3b8e8945aacc598f3e8b0) |
| James Hawkins | 2006-12-05 | [msi: Initialize sid\_str to NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b652fe8c65d056ed761b59f9e79c848b44a704d) |
| James Hawkins | 2006-12-05 | [msi: Fail if stg is NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=00fa70dbc1cdced835f559a847f8dd325334a25d) |
| James Hawkins | 2006-12-01 | [msi: Set the UserSID property.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8ae81d0620a0c11febea41fdfd463f692e506dbc) |
| James Hawkins | 2006-12-01 | [msi: Add handling for the StartServices action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=58bb3571defcde50770dc214608b890ab932b8f7) |
| James Hawkins | 2006-12-01 | [shell32: Move a NULL pointer check before the place where we dereference the pointer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=44b0b462cbbc118ce4b372dfecfb4f5f902b4e03) |
| James Hawkins | 2006-11-30 | [msi: Use mi-&gt;source if the source is not a full path.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a64945baeab3f6ccf41494dba078b16c92fde3bc) |
| James Hawkins | 2006-11-30 | [advapi32: Add tests for LookupAccountName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19a49eb51afbe860ca2614c58589f6f915124ddd) |
| James Hawkins | 2006-11-30 | [advapi32: Remove redundant NULL checks before CRYPT\_Free.](http://source.winehq.org/git/wine.git?a=commitdiff;h=024237efaaaa689d077b299016e0dedea541b722) |
| James Hawkins | 2006-11-28 | [msi: Add handling for the InstallODBC action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3bec325007ea60ae041ed17d750162e0cdb2f91) |
| James Hawkins | 2006-11-28 | [msi: Don't fail if we can't remove an existing install file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7125d3073d297f1b9a53d60958012ec59e3ca475) |
| James Hawkins | 2006-11-18 | [kernel32: Replace magic numbers with descriptive defines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15fd7a028fb277514db870c62cc1a8b9b2ad5432) |
| James Hawkins | 2006-11-13 | [msi: Notify the external UI handler when changing media.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31a9b087c15b7798d7c5b7766f151522add47028) |
| James Hawkins | 2006-11-10 | [msi: Fix a heap corruption bug by resizing the src string before adding to it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5cc4a8915f5b9873c16a2c2b6465d795fb05d019) |
| James Hawkins | 2006-11-08 | [msi: Add support for continuous cabinets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa8fc1628a455928f36e5dc884f87ad22a717fb4) |
| James Hawkins | 2006-11-08 | [msi: Move the file sequence check out of ready\_media\_info to avoid an unnecessary ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d21e1cc05bfbedc651b9c188f854fdb595f6ef1d) |
| James Hawkins | 2006-11-08 | [msi: Use disk\_prompt from the media\_info structure instead of passing an extra parame ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a621c2a6619ec43a1b33c4464e13864739c366cb) |
| James Hawkins | 2006-11-08 | [msi: Only add text to the scroll control if text is provided.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9d899129bf696afabf76ef5ba6f24fcf582abff7) |
| James Hawkins | 2006-11-08 | [msi: Factor out load\_media\_info from ready\_media\_for\_file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ef6512938d1162114735a482572755f9dd4d099) |
| James Hawkins | 2006-11-08 | [msi: Extract cabinets in ACTION\_InstallFiles. ready\_media is for finding and loading ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d537a311fb44edcdbca170ffab31ead2df73ebd) |
| James Hawkins | 2006-11-07 | [msi: Model the media\_info structure members after the columns in the media table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=de3b84df091ab13a6685f34fb905b38260e4b1d3) |
| James Hawkins | 2006-11-07 | [msi: Use the media\_info structure instead of passing in individual values to extract ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=b81f1ce561f31bf6ae729ba052e3b29508ae3924) |
| James Hawkins | 2006-11-07 | [msi: Store the base URL of the MSI package if it is downloaded.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae18c2dc7f7e337b0eb7f3a15f04d35a56355586) |
| James Hawkins | 2006-11-07 | [msi: Factor schedule\_install\_files out of ACTION\_InstallFiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a13bbaf7361830638c9e34c8a57bb2d955dae966) |
| James Hawkins | 2006-11-07 | [msi: Use the file's component instead of passing an extra parameter to set\_file\_source.](http://source.winehq.org/git/wine.git?a=commitdiff;h=988509e1afe1a1993c6c2fc336cff3dde3a06e38) |
| James Hawkins | 2006-11-07 | [msi: Add more tests for installing from cabinets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=84f34ec2101106320263c8df6229c7cccf7a66f0) |
| James Hawkins | 2006-11-07 | [msi: Use msi\_alloc\_zero instead of a helper function that sets everything to zero.](http://source.winehq.org/git/wine.git?a=commitdiff;h=842ffc35456fa447a9653b60938d68e845cc444b) |
| James Hawkins | 2006-11-07 | [msi: Factor copy\_install\_file out of ACTION\_InstallFiles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=542101fcda71016022fca5a8040acefec7878f01) |
| James Hawkins | 2006-11-07 | [msi: Factor out download\_remote\_cabinet and reuse extract\_cabinet\_file to extract ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ae4ab6ef7b911199c65dabd10be49657aeccb42) |
| James Hawkins | 2006-11-01 | [advpack: Use the full path of the INF file as the source directory if the CAB file ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a27ae7929566f42ee3dd420af7f284b57510d98b) |
| James Hawkins | 2006-10-27 | [msi: Implement handling for the ErrorDialog and use it to change media.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c6bfbde849b5ddf2217f30bbac31bc7e43043278) |
| James Hawkins | 2006-10-27 | [msi: Extract cabinets based on DiskId, not LastSequence.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62dc9ca691ea1449dc217351dc6ea7f9ca33ce17) |
| James Hawkins | 2006-10-27 | [msi: Test the order in which cab files are handled in the Media table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=005c0a792ea48a1e95b321d9a2a3c70c1973959d) |
| James Hawkins | 2006-10-26 | [msi: Add tests for the UPDATE sql command.](http://source.winehq.org/git/wine.git?a=commitdiff;h=62aedea856037208e93e36dcc5b7e6cc737b62e8) |
| James Hawkins | 2006-10-24 | [msi: Remove two unnecessary install tables.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a93763ae21ae73dd9bf252d769a8ce31ccd02833) |
| James Hawkins | 2006-10-24 | [msi: Remove unused function pointer and definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3a3d6c2547b36892f7dbc9ffe7a2806b87edb0e) |
| James Hawkins | 2006-10-24 | [advpack: Fix the full path check.](http://source.winehq.org/git/wine.git?a=commitdiff;h=615d09f285015e392c66c5873e97c871323f9144) |
| James Hawkins | 2006-10-24 | [msi: Add support for localizable strings in MsiDatabaseImport.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b19cc79bd4c35f1710280e569ec2847597b679c) |
| James Hawkins | 2006-10-24 | [msi: Allow more customization of install test files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3fc13d4b051bd7189e8d8af85996dad755759566) |
| James Hawkins | 2006-10-24 | [msi: Add tests for installing from continuous cabinets.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1f3f88bf67d32983ff00d96bf58bf91c6e72ae02) |
| James Hawkins | 2006-10-20 | [msi: Add tests for integer column types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcd57a3fc4e8a2a0664ba280a4fc570009aa30ee) |
| James Hawkins | 2006-10-20 | [msi: Allow more than one primary key in a table when importing a database.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a66584e1a26b4bc12ec0ae1befa87fdd67aa0b84) |
| James Hawkins | 2006-10-20 | [msi: Integer columns can have the 'NOT NULL' modifier too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=279f8158f8b96e992f18441822cbce24df855760) |
| James Hawkins | 2006-10-19 | [msi: Implement the InstallServices action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9bc12ade13d6ac69ecce7a40e5682516a36c2f1b) |
| James Hawkins | 2006-10-19 | [msi: Only initialize a component's state if it is linked with a feature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=929395c0f0b7dbd1978adfea5079445228b6b7e8) |
| James Hawkins | 2006-10-19 | [msi: Use the ProgramFileDir reg value instead of ProgramFilesPath.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7330a03200d7b91150a21ed6bdf41c64548cf2bd) |
| James Hawkins | 2006-10-18 | [msi: Add tests for the InstallServices action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d6632dd0fbcdcfc9e8b36d3e2dc048ae3c37cfa2) |
| James Hawkins | 2006-10-18 | [msi: Run SetProperty events before all other events no matter what the order is.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8321276cd34486bc6bf1e07c0e99c73423288854) |
| James Hawkins | 2006-10-18 | [tools/wine.inf: Add the ProgramFilesPath registry entry.](http://source.winehq.org/git/wine.git?a=commitdiff;h=463cec6af69a07adb59de376427bbb2079099293) |
| James Hawkins | 2006-10-18 | [msi: Set the USERNAME and COMPANYNAME properties when initializing a package.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08831b4a1e38afa8a5f56da6deef1527df4bbb50) |
| James Hawkins | 2006-10-16 | [msi: Revert &quot;msi: Perform button control events in greatest to least order.&quot;](http://source.winehq.org/git/wine.git?a=commitdiff;h=9119b700ed241391b6c52aecb697713bce529eee) |
| James Hawkins | 2006-10-13 | [mscoree: Add stub implementations of CorBindToRuntimeHost and GetCORVersion.](http://source.winehq.org/git/wine.git?a=commitdiff;h=eb676fff06ef702c6033f65edb7d39ebe31040ea) |
| James Hawkins | 2006-10-13 | [mscoree: Add missing stubs to the spec file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b2f21fa0710dd6771e2ee6886bd1172dfcb9ab50) |
| James Hawkins | 2006-10-13 | [clusapi: Add the clusapi.h public header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3cb50048760afefc61d8dcb6df599a857bb069c4) |
| James Hawkins | 2006-10-13 | [include: Move cfgmgr32.h to include/ to match the SDK.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b6017ae1894648f478ab242207e1153c20c8b57) |
| James Hawkins | 2006-10-13 | [msi: Also set the SOURCEDIR property in MSI\_InstallPackage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3797e6cadaf9fa1cb8e0995a06c79d71e217d35f) |
| James Hawkins | 2006-10-11 | [cabinet: Make internal functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e981278769600d3993ef029603d18d0d9d2c095d) |
| James Hawkins | 2006-10-11 | [crypt32: Make an internal function static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d813d8db1b144266cc6a5b247353c074af0f2644) |
| James Hawkins | 2006-10-11 | [advapi32: Add missing declarations to the public headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cdd717bc1bc0a85b204d880400b37675238877c4) |
| James Hawkins | 2006-10-11 | [comctl32: Make internal functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cd073a66a5ef6904acd0bec4ad43024ecd1655e6) |
| James Hawkins | 2006-10-11 | [gphoto2.ds: Make an internal function static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c9384a20329767b4aaface9c37943e8a71a83802) |
| James Hawkins | 2006-10-11 | [advapi32: Make internal functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2730fe6d1cdcf91ea5910ef8663d9093b892983a) |
| James Hawkins | 2006-10-10 | [msi: Set the SourceDir and SOURCEDIR properties in the ResolveSource action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c507543554b519f0dc3c50756c7c207f0c9e988a) |
| James Hawkins | 2006-10-10 | [msi: Clean up after the package tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=58870ce841f71d162277360930e82841a1729069) |
| James Hawkins | 2006-10-09 | [msi: NULL-terminate dst on error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=915898fbb75b8f2f945f4934d3b67496d3073558) |
| James Hawkins | 2006-10-09 | [advpack: Make internal functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b9ad4d3bc04f126e40e679dcf3d58b3e35dcc05) |
| James Hawkins | 2006-10-09 | [msi: Add missing declarations to the public headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5fd3c4ad15bfe7f976ca421c81f285487ddced29) |
| James Hawkins | 2006-10-09 | [msi: Make internal functions static.](http://source.winehq.org/git/wine.git?a=commitdiff;h=563a50ab357049b15a84951397699f783e907711) |
| James Hawkins | 2006-10-09 | [msi: Add missing sizeof(WCHAR) multiplier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=42b05ea311514414198293b609b96435877739ba) |
| James Hawkins | 2006-10-07 | [msi: Perform button control events in greatest to least order.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f721a24a13bf250f0794b7249ffa863619b0b450) |
| James Hawkins | 2006-10-07 | [shdocvw: Return S\_OK in PersistStorage\_InitNew.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e55ed113faee6c3d52cdd5043069f041c34c7bc0) |
| James Hawkins | 2006-10-07 | [janitorial: Remove redundant NULL checks before CoTaskMemFree (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=99e2c6dff20f1692d70073b38e8fad43722269ed) |
| James Hawkins | 2006-10-07 | [janitorial: Remove redundant NULL checks before SHFree.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7b89ff88e85a95f1e16420d25654887c71adcc6b) |
| James Hawkins | 2006-10-07 | [advpack: Win64 printf format warning fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29a55bd512267af743a2ccbc8833750d03678c42) |
| James Hawkins | 2006-10-06 | [advapi32: Remove redundant NULL check before SERV\_free (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca118989f454554f6913337cca272a925653d0db) |
| James Hawkins | 2006-10-06 | [crypt32: Remove redundant NULL checks before CryptMemFree (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=b96ac007645c94c8f44ec8983f53c5b4a247cb43) |
| James Hawkins | 2006-10-06 | [msi: Make msi\_dialog\_dup\_property return a copy of the property if the property is ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=9024a88dd996887a34d10b39231971b22f703143) |
| James Hawkins | 2006-10-06 | [dinput: Call missing LeaveCriticalSection in the error case (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=553bafd535c2dbbc5f2a49b423982285c35112e1) |
| James Hawkins | 2006-10-06 | [dbghelp: Remove redundant NULL checks before pdb\_free (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=1b95f6093868254b612138ae1136d2257a551b0f) |
| James Hawkins | 2006-10-06 | [ddraw: Set lplpDirect3DViewport3 to NULL before returning an error (found by Smatch).](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a922b6a3887d89a767af46aef94d7d10acb4ed2) |
| James Hawkins | 2006-10-04 | [msi: Only apply the last font style in the list of styles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f16ddf1b325b2e2b57b4bd940b7372135b968d00) |
| James Hawkins | 2006-10-04 | [user: Add missing sizeof(WCHAR) multiplier.](http://source.winehq.org/git/wine.git?a=commitdiff;h=96963d2bc18aa8fc46aad623c6c122cfa8e4054c) |
| James Hawkins | 2006-10-03 | [msi: Assign the property to path if the property is empty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e3496be256a563c97e91871ef21f149bae4d63be) |
| James Hawkins | 2006-10-03 | [msi: Properly initialize the SelectionTree control's attributes and property values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=de0efba366ede0f1f3cd62fc114aefe51ebe05fc) |
| James Hawkins | 2006-10-03 | [msi: Publish the SelectionPath event in the SetTargetPath event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aea0dcc86da5c4779c04c87e4db7c9d409c7d739) |
| James Hawkins | 2006-10-03 | [msi: Handle the SelectionBrowse event using ControlEvent\_SpawnDialog.](http://source.winehq.org/git/wine.git?a=commitdiff;h=971ab9aa47476a56a1d6ee616fa332351c368f7b) |
| James Hawkins | 2006-10-03 | [msi: Store the selected item in the SelectionTree control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=908e27d6fcb8cb874912d610b6e5f9c311e721e8) |
| James Hawkins | 2006-10-03 | [msi: Publish the SelectionDescription and SelectionPath events when the selection ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=846fdd1550925803f1613fdad02f00bc1a4ddddd) |
| James Hawkins | 2006-10-03 | [msi: Select the first item in the SelectionTree control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7ee3a4efdf13b671dcf253fd4265d2d7f41944f1) |
| James Hawkins | 2006-10-03 | [msi: Subscribe the SelectionTree control to the SelectionPath event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ea2cd44c1766710bf6c944a1889e1e47c8bd15d) |
| James Hawkins | 2006-10-03 | [comctl32: Set the TVIF\_TEXT mask when notifying the parent window of a selection ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d2b37cc8391f9f02f6405649f33492adf1242b0) |
| James Hawkins | 2006-10-03 | [msi: Provide a specific dialog to ControlEvent\_SubscribeToEvent, as package-&gt;dialog ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a8c38ff74f0ba488934cdb0fd30fce3139ab43e) |
| James Hawkins | 2006-10-03 | [msi: Add missing '\n' to TRACE output.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1bfc50eb74f7a434039db54e78737d74062053f7) |
| James Hawkins | 2006-10-03 | [msi: Empty the window text if no text is provided.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0fe1b3671624ceb077598eac8f7deaa24469a671) |
| James Hawkins | 2006-10-03 | [msi: Don't ERR if a dialog doesn't provide control conditions, as they are not required.](http://source.winehq.org/git/wine.git?a=commitdiff;h=038d31ca93f0fee8af13b5863d3da07536de0945) |
| Benjamin Arai | 2006-09-29 | [resutils: Implements stub dll for resutils.dll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ac07aa0164a9e2923998789d77f6e7f20501d35) |
| James Hawkins | 2006-09-28 | [msi: A feature state of INSTALLSTATE\_ABSENT translates into a component state of ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=d83aa64c57072fad6960076ce3aab830e2cfe639) |
| James Hawkins | 2006-09-28 | [msi: Follow state resolution rules when a feature parent saves a component.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cabc7ee1ae327e4e29c3f9910498d83f48e56af7) |
| James Hawkins | 2006-09-28 | [msi: Implement MsiDatabaseImport.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6be7ba7546f9d38ca0d3b6006ff4895dad4d83fd) |
| James Hawkins | 2006-09-28 | [msi: Return to the parent dialog when the argument to the EndDialog event is Return.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d812659e87c472a81a152f2ddfe27bd18801deb) |
| Benjamin Arai | 2006-09-27 | [clusapi: Implement stub dll for clusapi.](http://source.winehq.org/git/wine.git?a=commitdiff;h=493bc6b875d8c0c41e9a22da2c420216d4490c73) |
| James Hawkins | 2006-09-26 | [msi: Store the full path to the database file in the MSIDATABASE structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=da14a4a25e686c5395164fb82c60d7b9590e7d50) |
| James Hawkins | 2006-09-26 | [msi: If the feature linked to a component has a state of INSTALLSTATE\_UNKNOWN, the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=bbd4d1e3ef314098f1e7777629cb0bc7c347c330) |
| James Hawkins | 2006-09-26 | [msi: Only specifically resolve the TARGETDIR directory once.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad609f15180b73f75f08d7e61223f70294befb71) |
| James Hawkins | 2006-09-26 | [msi: Add tests for setting the target path of TARGETDIR (based on a patch by Andrey ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ee3fc35ef9d2a3173b01b3bd925dc55a21bd7f3) |
| James Hawkins | 2006-09-22 | [setupapi: Fix a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5dadca4dbca70cd98db68f1fb2d5fa0c8348a636) |
| James Hawkins | 2006-09-21 | [msi: Load the component states in CostFinalize instead of CostInitialize.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d893cb7d1e1f52bf5e156f347e6300ccc449d7f9) |
| James Hawkins | 2006-09-21 | [msi: Initialize all features' action states to INSTALLSTATE\_UNKNOWN.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca5c11009da675aae6407bcf5c74f57baab4d128) |
| James Hawkins | 2006-09-21 | [msi: Only override a feature whose action state is INSTALLSTATE\_SOURCE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=937b9b2bbc0c2a264f124ddb5bd5e921e9eded02) |
| James Hawkins | 2006-09-21 | [msi: Translate the INSTALLSTATE\_UNKNOWN index into the INSTALLSTATE\_ABSENT image ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=703d77dc58a032b08dc222de951474a7f28f8fac) |
| James Hawkins | 2006-09-21 | [msi: Fix the results of a few tests to match Windows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ac0f3ed29802487898623d256a6906786416556) |
| James Hawkins | 2006-09-21 | [msi: Disable child features of parent features that are unselected because of the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=545d0e70cf200270956193f6606eb2a9cbb2933a) |
| Benjamin Arai | 2006-09-21 | [msi: Adds test to check &quot;JOIN&quot; operator with &quot;\*&quot; operator for the SELECT clause retur ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=4195697cc1405ecc9de4bb0d10790bbf4d37dd32) |
| James Hawkins | 2006-09-21 | [msi: Don't check a component's install state if a component ID is not provided.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32f570222be9e96b0e1730a4686163413451af95) |
| James Hawkins | 2006-09-21 | [advpack: backup should be a const string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=319cac4c1fd497ba68445201b95278417b5cfd22) |
| Benjamin Arai | 2006-09-20 | [msi: Adds test to check if &quot;AND&quot; operator returns the correct result for the &quot;WHERE&quot; ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=f84c1463c1325528f6c664f3b369de3861a03cc2) |
| Benjamin Arai | 2006-09-20 | [msi: Adds test to check if basic &quot;JOIN&quot; operator without &quot;WHERE&quot; clause returns the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=a35ff56580329de3a1dc2aa47029568550c23ba6) |
| Benjamin Arai | 2006-09-20 | [oleaut32: Conformance test for function variant:VarImp.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8d921f1d3cc0dac880e78817745f8255b9123aa3) |
| Benjamin Arai | 2006-09-20 | [oleaut32: Implementation for function variant:VarImp.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4cb6c9184b24f9be421306f15f9d1a05515c90a3) |
| Dan Hipschman | 2006-09-20 | [msxml3: Fix IXMLDOMNamedNodeMap\_getNamedItem() conformance on error.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47b6d3a1e3a19796eb8b5a4578eba48a7fb23401) |
| Benjamin Arai | 2006-09-19 | [msi: Updates tests for joins to include row and column ids in message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4c6b06ed7d73c63d9e9de7e6dd878594c85eaa7) |
| Benjamin Arai | 2006-09-19 | [msi: Adds tests to check if joins return the correct number of rows.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32d002c7ed166348f62e613cf9784dbfcfd78e02) |
| James Hawkins | 2006-09-16 | [msi: Add tests for components with multiple parent features.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4c6ca2b6551f822733284041b6bf8768b69bab4) |
| James Hawkins | 2006-09-16 | [msi: Use ACTION\_UpdateComponentStates in the selection tree so we don't have to dupli ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a97b3ed84baf36d7a09f5932d64f4daa819a890) |
| James Hawkins | 2006-09-16 | [msi: INSTALLSTATE\_SOURCE also overrides a parent feature state change to INSTALLSTATE ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=6518f3d7f2515b52a9c0d2f8a757998b41bd2ead) |
| James Hawkins | 2006-09-15 | [msi: Add the total and free disk space to the VolumeCostList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=32c0a764ee898349b1278eab196e17b59fe1c1aa) |
| Benjamin Arai | 2006-09-15 | [nddeapi: Implement stub dll for nddeapi.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b4eafada9e1b484c19ea99e64aeb57fea405478) |
| James Hawkins | 2006-09-14 | [wintrust: Add a stub implementation of CryptCATEnumerateMember.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ab5494e83ecde54f37ec02cf9fd20219d12baab1) |
| James Hawkins | 2006-09-14 | [wintrust: Add a stub implementation of CryptCATOpen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a89db155d8aa9e70216ee8baae921deca653a8a0) |
| James Hawkins | 2006-09-14 | [wintrust: Move the Crypt\* functions to crypt.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8082477d6c0cdc3a413ad97515679cbb8aa53ad4) |
| James Hawkins | 2006-09-14 | [wintrust: Add a stub implementation of CryptCATClose.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15b7934f3da0ccb2afc0976248a504fad2ca36d2) |
| James Hawkins | 2006-09-14 | [setupapi: Add stubs for SetupOpenLog, SetupCloseLog, and SetupLogError.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15b46847b0bc4d9bcc2b03d9377ce7342f4da536) |
| Dan Hipschman | 2006-09-13 | [widl: Remove unused parameter in create\_msft\_typeinfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd7e690c1fbdf68cc8220e1a91b706ad946bc9cc) |
| Dan Hipschman | 2006-09-13 | [widl: Add -u and -U options to man page.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a472c83f9174e82ecd91dc37728afeba5a661fd5) |
| Dan Hipschman | 2006-09-13 | [widl: Replace a #if by if for better compiler checking.](http://source.winehq.org/git/wine.git?a=commitdiff;h=954c592a6c076626e2789415f86612404d30f8a1) |
| James Hawkins | 2006-09-13 | [setupapi: Implement pSetupGetField, with tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7588b669d8331ff64fc3b75cebe40ef518cd0de1) |
| Dan Hipschman | 2006-09-13 | [widl: Remove unused parameter in write\_ip\_tfs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6e7389ada8a7942031399a8763efa82eeb2ddfad) |
| Dan Hipschman | 2006-09-13 | [widl: Fix warning about unused structure field in lexer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53a28192865d212021ff4f3a573dd78f80584be0) |
| Dan Hipschman | 2006-09-13 | [widl: Remove unused parameter in ctl2\_encode\_name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=48006f60a7462d889264a1c4839de015ee481cc1) |
| Dan Hipschman | 2006-09-13 | [widl: Don't compare result of read() to unsigned type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ad3f8de42658db331110bf14baa5b81be6c809a) |
| James Hawkins | 2006-09-12 | [msi: Add more join tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bfc1b5c15f35237e4234fca29f98079d59c4d69c) |
| Dan Hipschman | 2006-09-12 | [oleaut32: Replace a loop with a simple computation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b6e6d4b5115ff46c76ad390bb518bc50df09c7cb) |
| James Hawkins | 2006-09-12 | [msi: Show the available drives in the VolumeCostList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=75ee2262cc3f49e7718cb114ae159bf3eaf6d167) |
| Dan Hipschman | 2006-09-12 | [widl: Replace a loop with a simple computation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6f4b83bce07100bdef792238260c66a1fa6bd589) |
| Benjamin Arai | 2006-09-11 | [oleaut32: Fixes for function variant:VarIdiv.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed6499918058bc274357cd9b24081f14d84f8eee) |
| Benjamin Arai | 2006-09-11 | [oleaut32: Fixes for function variant:VarDiv.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aaca30cf039c227ef03268e10abdea3afbe239f8) |
| Benjamin Arai | 2006-09-11 | [oleaut32: Conformance test for function variant:VarDiv.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a4ec2721a48508d672f2d7ca3c1b2d4d44836f4e) |
| Benjamin Arai | 2006-09-11 | [oleaut32: Conformance test for function variant:VarIdiv.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e1f392a273b5a580c90cd599d5581db554f4a18) |
| James Hawkins | 2006-09-11 | [msi: Don't try to register a class if a COM server file is not provided.](http://source.winehq.org/git/wine.git?a=commitdiff;h=61db539cec1e44927b1c8ea8bf2d8c948800bd80) |
| Benjamin Arai | 2006-09-08 | [oleaut32: Fixes for function variant:VarPow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fbf9cba6833701ddcd201138dec1ad0d6c1ee756) |
| Benjamin Arai | 2006-09-08 | [oleaut32: Conformance test for function variant:VarPow.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aee8a62136f51b1784f271cb0aaecfc9fa806f6f) |
| James Hawkins | 2006-09-08 | [msi: Allow non-key columns to be used with the join query.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a302f03c6533abec30e6664e6e152d167000b773) |
| Benjamin Arai | 2006-09-08 | [oleaut32: Conformance test for function variant:VarAnd.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e3e591bf24d4adcf3ce9aefb68eaad9c29f0009) |
| Benjamin Arai | 2006-09-08 | [oleaut32: Fixes for function variant:VarAnd.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3abb454c707ad6cb91dc23cb59e5ca5a5871bac2) |
| James Hawkins | 2006-09-07 | [msi: Add tests for MSI SQL join queries.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d8c13370b31d067c9edab7770cae31ee036652fa) |
| Dan Hipschman | 2006-09-07 | [widl: Add more complete pointer handling to write\_typeformatstring\_var.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ff8ae327f783252407192c5ac431ec13f8e0db8) |
| James Hawkins | 2006-09-06 | [msi: Use the TargetPath of a file if the file doesn't exist in MsiFormatRecord.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ff6fe41df74a244282e8d38369d4d8da37141dba) |
| James Hawkins | 2006-09-06 | [msi: Add many more MsiFormatRecord tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f6463dfacdad2a1f6d0f12660c1b0a712a5176ed) |
| James Hawkins | 2006-09-06 | [msvcmaker: Remove a reference to libs/unicode in msvcmaker.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bedcdee7147d448af47193cca1ec65d20576f3c2) |
| James Hawkins | 2006-09-06 | [msi: Fix creation of the default format in MsiFormatRecord.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a248cc8f6284754c4b1abbe35ba42465437eb0b0) |
| James Hawkins | 2006-09-06 | [msi: Fix two MsiFormatRecord tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16769b26b2bbd7adbca85eb93fe9b2c4dcd944f3) |
| James Hawkins | 2006-09-05 | [msi: Add more tests for MsiFormatRecord.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad2ec01739dd8eaa565591a4b6888f3b4259002d) |
| James Hawkins | 2006-09-04 | [msi: Add the ability to change directories in the DirectoryList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4969ccf3af4a72d93ae13043f50f0123d37ab989) |
| Dan Kegel | 2006-09-04 | [programs/wcmd: Rename to programs/cmd.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39857443e4159d5c9e04fb93e158603b374f1a44) |
| James Hawkins | 2006-09-04 | [msi: Store the CustomActionData for deferred custom actions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0405e9d2d438878ab52bf6c0c52f522410163f0b) |
| Dan Hipschman | 2006-09-01 | [widl: Sanity check string and pointer attrs.  Don't assign string as type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a407da47751912ff7ea4adad2e915c6357d0eb1a) |
| James Hawkins | 2006-09-01 | [msi: Load and display the VolumeCostList control's column headers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f691adf7e4ac27d8ea0f45ca19b9b695244ffc7) |
| Dan Hipschman | 2006-09-01 | [widl: Handle more pointer types in get\_struct\_type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=180ede5bfee6502a1950405d4cc17fe4941cf57c) |
| James Hawkins | 2006-09-01 | [msi: Add initial implementation of the DirectoryList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01432d71652857bbd0fc506b20718941e96613d2) |
| James Hawkins | 2006-08-31 | [msi: Verify the path in the PathEdit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad559ca86d8a48e8aebeed326d360edf5306d05f) |
| James Hawkins | 2006-08-31 | [msi: Search for the browse dialog controls by type instead of name.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c3e640c100b90a928de7d9f45ab176dd88c7631) |
| James Hawkins | 2006-08-31 | [msi: Add more tests for the \_Streams table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e86590518504b8c9046db5b080150f5f85eefb0) |
| James Hawkins | 2006-08-31 | [msi: Provide the control to the dialog\_update function for the case](http://source.winehq.org/git/wine.git?a=commitdiff;h=4e3f6eda0e3af2a226e50044dca7baf9f97e479f) |
| James Hawkins | 2006-08-31 | [msi: Store and use the center point of the dialog window in between dialogs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1cfdc5185a86934b634674e7ff4654b4367aedca) |
| James Hawkins | 2006-08-30 | [crypt32: Simplify CRYPT\_AsnDecodeNameValueInternal, getting rid of a warning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a9670e371e8d582147980a743c0073e95e5ac8ea) |
| Dan Hipschman | 2006-08-30 | [widl: Remove checks for typedefs that always fail.](http://source.winehq.org/git/wine.git?a=commitdiff;h=88820263c6ed440a0dcadefb6b1dd2316c20404a) |
| James Hawkins | 2006-08-30 | [crypt32: Simplify CRYPT\_AsnDecodeUnicodeNameValueInternal, getting rid of a warning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=382d06794b40391b0cf7961dec89260735897dde) |
| James Hawkins | 2006-08-29 | [advpack: Get the proper working directory in install\_init.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5acc51f2c495e32305a72de30fea82fd6f19379) |
| Dan Hipschman | 2006-08-29 | [widl: Use type\_t for typedefs, not var\_t.  Simplify representation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c117a20cdb5ffbe04fd334bd7139fdb9dd60978a) |
| Dan Hipschman | 2006-08-29 | [widl: Factor the entry\_t structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=aadc90b2668ea641d4ed7dfba2b9f24f125f73b1) |
| James Hawkins | 2006-08-29 | [advpack: Add the regsvr action to the SetupInstallFromInfSection call.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a39913fa1199ff2bf1c2c7602ce688eea2295483) |
| Dan Hipschman | 2006-08-29 | [widl: Add an is\_ptr function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=929a75989594cbc5e47772b36d89def30a5546e7) |
| Dan Hipschman | 2006-08-29 | [widl: Print pointers more aesthetically in generated header.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7e79e9d4fff058d95e45ed16fe514b20b54c4884) |
| James Hawkins | 2006-08-29 | [msi: Highlight the text in the PathEdit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7df642117c2e23949a329ba6d070f7078427c0fe) |
| James Hawkins | 2006-08-29 | [msi: Update the DirectoryCombo control in response to the DirectoryListUp event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6320d0adef3003d3bc941856c29c6bbb41f09df8) |
| Dan Hipschman | 2006-08-29 | [widl: Generate names for tagless structs, unions and enums.](http://source.winehq.org/git/wine.git?a=commitdiff;h=59cfad37aab59d307383f828d1ca79275efad453) |
| James Hawkins | 2006-08-29 | [msi: Update the PathEdit control in response to the DirectoryListUp event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2dbaccbe606f7a1ddec13717ccb93f28457d9355) |
| James Hawkins | 2006-08-29 | [msi: Use the respective update functions when creating the Browse dialog control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a09d4f6c722e400a0fc7473d8c7ff1c792e3b07) |
| James Hawkins | 2006-08-29 | [msi: Use msi\_dialog\_dup\_property where appropriate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=20d98e81eda835a91524f2585f3253a806b968a5) |
| Dan Hipschman | 2006-08-29 | [widl: Generate an error for &quot;int f(void a)&quot;.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1687a5d1db2c0bcd3f7155c6195d500b7959010b) |
| Dan Hipschman | 2006-08-29 | [widl: Add the rest of the pointer types to write\_type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=04a15af5dc9e0f68b1ee0cad2dbf8b9d642b35e0) |
| Dan Kegel | 2006-08-28 | [msi/tests: Add test to verify we can create 4000 msi handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98ec9399c4ac33b84b6ff88338722e83f379d427) |
| Dan Kegel | 2006-08-28 | [msi: Callers of alloc\_msihandle should handle failure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=337e1e202f636404933cbb721366306f0d59b788) |
| Dan Kegel | 2006-08-28 | [msi: Remove limit on number of handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=29f0803c0239fe2495ffddd96471cd03475dc0db) |
| James Hawkins | 2006-08-25 | [msi: Add initial implementation of the DirectoryCombo control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a97962eef442016f4e2f550bdaede236a47c9925) |
| James Hawkins | 2006-08-25 | [msi: Add initial implementation of the DirectoryListUp event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1b16d2d96c7d7e29bf9fd7dfccd45436242ea5e) |
| Dan Hipschman | 2006-08-25 | [widl: Remove usage of type\_t ref field for base types; simplify code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=94755218aca1e1597f2b1a5562e1b71cfad13259) |
| James Hawkins | 2006-08-25 | [msi: Add a stub implementation of the VolumeCostList control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=80225d53b945caa68b58f4f67cd9c512ebacbcc7) |
| James Hawkins | 2006-08-24 | [msi: Inform the user with an error message when the MSI file path is invalid.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fb7646beaa1a76f40ed0e05ab0dd7c36034439b7) |
| James Hawkins | 2006-08-24 | [msi: Add a stub implementation of the DirectoryCombo dialog control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c9674e690c053c4be05e4b651909e7702d18f442) |
| Benjamin Arai | 2006-08-24 | [oleaut32: Updated conformance test return string for VT\_RESERVED.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6aaf2af5c0b95d7599bfc02425f0961b96504dcf) |
| James Hawkins | 2006-08-24 | [msi: Add a stub implementation of the DirectoryList dialog control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=25062556a8f06c5064904a0096ddddda2bdd0957) |
| James Hawkins | 2006-08-24 | [msi: Add an initial implementation of the PathEdit control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=11b7097df8b12b4a4b7bd6485365089d502f9cec) |
| James Hawkins | 2006-08-24 | [msi: Fix the height of the line control window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0de9cf4d002964eef7b2c4fa51c6e7e478286e09) |
| James Hawkins | 2006-08-23 | [msiexec: Add handling for msiexec's regserver option.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a6b8ff9ddbf4ee03e570d9e3b7ec925b34cc0361) |
| Benjamin Arai | 2006-08-22 | [oleaut32: Add support for handling TKIND\_COCLASS in userdefined\_to\_variantvt.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1282dce887f2c17d99a633a59fda81bb17d78f5) |
| James Hawkins | 2006-08-22 | [msi: Add tests for the AppSearch action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=80740e72e7410a7560644fa83b8af3c20802441d) |
| James Hawkins | 2006-08-21 | [msi: Add tests for MsiEvaluateCondition's substring operators.](http://source.winehq.org/git/wine.git?a=commitdiff;h=762a13eb348010b140f3c779e0a0147dd87fd979) |
| James Hawkins | 2006-08-21 | [msi: Add handling for MsiEvaluateCondition's substring operators.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a520c0b6d6eb92c92f8172e58f41e01d7c59032) |
| Dan Kegel | 2006-08-20 | [mpr: Fix bug in ProviderOrder comma processing in wnetInit().](http://source.winehq.org/git/wine.git?a=commitdiff;h=50ed26c358e74a0380c9514792e0de6fb844ce27) |
| Dan Hipschman | 2006-08-18 | [widl: Allow format-string functions to work with objects.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b16916ed13e0b26ab3f375f2deb5cb146fda1b3) |
| Dan Hipschman | 2006-08-18 | [widl: Output format-strings for interface pointers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3870bf0d9e69924ac98633f5a0b541f77ec8f144) |
| Dan Hipschman | 2006-08-17 | [widl: Use typegen.c format-string functions in proxy.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed10b24e14cd13d68fa380683f805a617d67dabc) |
| Dan Hipschman | 2006-08-17 | [widl: Move format-string declaration output to typegen.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7e7243a1e5a4eb17c868246d075751fb1c1ac45) |
| Dan Hipschman | 2006-08-16 | [widl: Fix NdrComplexStructUnmarshall calls in generated code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e77a079b279ba168ab9d2d66390d2f2247edfafd) |
| Dan Hipschman | 2006-08-16 | [widl: Fix out-only temporary variable generation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c526c980d7ac68e0918c278bfccc50e118fe3ea9) |
| Dan Hipschman | 2006-08-16 | [widl: Fix NdrConformantArrayUnmarshall calls in generated code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b17d1c14d955fcce557010e5ee1cf777db919d32) |
| Dan Hipschman | 2006-08-16 | [widl: Generate proxy code for user marshalled types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a5ff173cc3dccbe63185420158fcc8a620a6cc1d) |
| James Hawkins | 2006-08-15 | [msi: Use the bare minimum number of parameters for LookupAccountName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4a27358a57ff2f398c63de6c2dc688ed8f06d7b) |
| James Hawkins | 2006-08-15 | [msi: Add a stub for MsiGetFeatureCost.](http://source.winehq.org/git/wine.git?a=commitdiff;h=485484deace78519bf7309030400fab0f4d3d2ca) |
| Dan Hipschman | 2006-08-15 | [widl: Calculate method indices in parser instead of during header generation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=16d4e712301e4e10159807ec261b321b4a2665d5) |
| Benjamin Arai | 2006-08-14 | [oleaut32: Conformance test for olefont:ReleaseHfont.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c4ba8a8c87b3fab44422546f70f1bf0dfc433fa4) |
| Benjamin Arai | 2006-08-14 | [oleaut32: Conformance test for olefont:AddRefHfont.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf6867024cb5ecd01429ba38ce79c1d4fda48354) |
| James Hawkins | 2006-08-14 | [msi: Non-compressed files may come before the list of compressed files in the file ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=75cc5f1e5e174d8a926b90a5eb004d5f6729e504) |
| Dan Hipschman | 2006-08-14 | [widl: Pass the right size to MIDL\_memset in generated proxy code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47519f08a706b81db78391768a6027eb6d116076) |
| Dan Hipschman | 2006-08-12 | [widl: Improve pointer null checking logic.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e49a8d2f2465030b1502031a8201354fa04f11d) |
| Benjamin Arai | 2006-08-12 | [oleaut32: Added test to check if olefont:IFont\_QueryInterface increments ref counter.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b44e9a64192c2244614dbb3dd42284f95c62dd0) |
| Dan Hipschman | 2006-08-12 | [widl: Use ref\_type to simplify some code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=06497dd44c2d9cacbfabe3384d2e7433675dc0e8) |
| Benjamin Arai | 2006-08-11 | [oleaut32: Removes stub message from olefont:OLEFontImpl\_FindConnectionPoint.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3dade1e7def970bffd0aeac5d34b831e1ea37ed1) |
| James Hawkins | 2006-08-11 | [msi: If a component's state is not local, source, or default, default to the local ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=3cb82ab8d29561637fe46a532ebca0d300cbfce2) |
| Dan Hipschman | 2006-08-11 | [widl: Don't generate indentation spaces on empty lines.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05001b1ca8bce4dce7c958e4732779706372cb62) |
| Dan Hipschman | 2006-08-10 | [widl: Fix incorrect version number in generated code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a20f7f46dcc032478e966c2301d05002440b8423) |
| James Hawkins | 2006-08-10 | [msi: Only remove a file if the version to be installed is strictly newer than the ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d37be9e56e9b875142a93a7af0671f2d9bc2947) |
| Dan Hipschman | 2006-08-09 | [widl: Add ref\_type (dereference typedefs) and use it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=216171fe523c053d4aa28f3e242f029d7632849d) |
| James Hawkins | 2006-08-09 | [msi: Download install cabinet files if the msi package is remote.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1ff96c63a82d8192454d3513a4e0110c1bc02026) |
| James Hawkins | 2006-08-08 | [msi: Add tests for the RemoveFiles action.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf4e00fd9bb0188df43d09720cf6ca4c5efb184a) |
| James Hawkins | 2006-08-07 | [msi: Fix the compressed files logic.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f84fa0ce6354827d6b2396ca3119c9a8bb7efcfb) |
| James Hawkins | 2006-08-07 | [wintrust: Always return ERROR\_SUCCESS in WinVerifyTrust.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5e0195be642117e0380db1bbdf8d1a55cb4e383) |
| James Hawkins | 2006-08-07 | [msi: Add tests for MsiGetProperty.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4fade6d3a85df6872d676d33fcee1a0666f8e73c) |
| Dan Hipschman | 2006-08-04 | [widl: Generate GUID (infile\_i.c) files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=df91150e10c093933bd4fd685a68885f38067b8e) |
| Dan Hipschman | 2006-08-04 | [user: Call SetLastError in CreateWindowEx when WS\_CHILD is set with no parent.](http://source.winehq.org/git/wine.git?a=commitdiff;h=74ece17c6bd141c5a13b3aec7522303fb50bc472) |
| Dan Hipschman | 2006-08-04 | [user: Add a test for CreateWindowEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=50486859706d01f5d639d8029a5cba71bdd9ccae) |
| Dan Hipschman | 2006-08-04 | [widl: Replace strdup, malloc and realloc with xstrdup, xmalloc and xrealloc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4961379d7408cc6f080106b0c01e85eb014da17d) |
| James Hawkins | 2006-08-04 | [msi: Use the initial dialog position values in the database when creating the dialog ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=23027f54356286907f5fec525059222a243284fd) |
| Benjamin Arai | 2006-08-04 | [oleaut32: Removes extra string allocation for varformat:VarMonthName.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0227b8cba228b17159a6ca392b801eda38815dca) |
| Dan Hipschman | 2006-08-03 | [widl: Write forward declarations for coclass definitions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=99056d7e2ac56e11a4f6c101463c705abb611bf1) |
| Thomas Kho | 2006-08-03 | [server: Remove unused thread\_apc member.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3538c0cdce81e1ee0861b0651da734aef14f0cfa) |
| Benjamin Arai | 2006-08-02 | [oleaut32: Implement function olefont:OLEFontImpl\_IsEqual.](http://source.winehq.org/git/wine.git?a=commitdiff;h=be37e9510568c5e6afd2ffd7de3a70a42aed5d13) |
| James Hawkins | 2006-08-02 | [msi: Add tests for SQL query markers.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91ec65d7f150a7951d4b17119447bfb9167bcaa2) |
| Benjamin Arai | 2006-08-02 | [oleaut32: Conformance test for olefont:OLEFontImpl\_IsEqual.](http://source.winehq.org/git/wine.git?a=commitdiff;h=41641554f4c4563a0c794375bc7ce60d13201c88) |
| James Hawkins | 2006-08-01 | [msi: Don't crash if an empty record is given to MsiProcessMessage.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f10365bb5dd9a0994368dfd82834691db5250598) |
| Thomas Kho | 2006-08-01 | [msi: Wake dialog on messages from external threads.](http://source.winehq.org/git/wine.git?a=commitdiff;h=88cc410fd62f51c52e052c1ca50a1380686ed513) |
| James Hawkins | 2006-08-01 | [msi: Set the install state to INSTALLSTATE\_LOCAL for features with compressed files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7edea0cc6868505252c65cbf0846b2f577660e51) |
| James Hawkins | 2006-08-01 | [msi: A file that does not have the msidbFileAttributesCompressed bit set should be ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=1dd97aa15428c0fc97a4f909f28f252f4d85723d) |
| Dan Hipschman | 2006-08-01 | [oleview: Initialize TVITEM.lParam to NULL in EnumFuncs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=10d552b22ef60a755584cf9e980c52beb8e50731) |
| James Hawkins | 2006-07-31 | [setupapi: Add a stub implementation of SetupGetSourceInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b74f4d92d74953eabb594a17c91fb6a6aff60ee7) |
| James Hawkins | 2006-07-31 | [msi: Set the install state to INSTALLSTATE\_LOCAL for components with compressed files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=98d148641046bba33845b11178b76be121ae2b0f) |
| Benjamin Arai | 2006-07-31 | [oleaut32: Move varformat conformance tests to new file varformat.c](http://source.winehq.org/git/wine.git?a=commitdiff;h=63c26dac23323d94599efe70caf86cf3ba61b7c2) |
| James Hawkins | 2006-07-31 | [msi: Fix the add\_feature\_entry helper function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6330f14da9d3a7519cb59e14a37f128d77f6dee4) |
| Thomas Kho | 2006-07-31 | [riched20: Implement EM\_GETLINE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f19ffe809aa68a2936ae6a3b0df677932fd0ef7) |
| Dan Hipschman | 2006-07-31 | [widl: Set type\_t kind field correctly for all types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3e1ace5aa32c2995cedb0f75e3635a4ef57da0ed) |
| James Hawkins | 2006-07-31 | [msi: Fix a couple install state test cases.](http://source.winehq.org/git/wine.git?a=commitdiff;h=38f2ba23f1a9f877f220e9776ad19f9d99492bd2) |
| Dan Hipschman | 2006-07-31 | [widl: Set defined flag for coclasses.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23707beb461c7c44a17088de4c78d4f654ca2091) |
| Dan Hipschman | 2006-07-29 | [widl: Fix &quot;static declaration follows non-static declaration&quot; in generated code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf4c08dcbc34ee1a9cbc68bcbf9b30da5eb09e69) |
| Benjamin Arai | 2006-07-28 | [oleaut32: VarSub: Conformance test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f10ed1f16eaac58e04bed943f608833269840f54) |
| Dan Hipschman | 2006-07-28 | [widl: Fold class\_t into type\_t.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c67b19b4f4bd463eedfbd4de77b846f9efb8a040) |
| Dan Hipschman | 2006-07-28 | [widl: Check if a typeinfo is already in a typelib before adding it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c650cceae32849ea974328a94753cd2cef94a9c1) |
| Benjamin Arai | 2006-07-28 | [oleaut32: VarSub: Fixes several data types and corrects error codes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9634ffa7dca3f42a7aeae9a9bb62c2bddf84e289) |
| Dan Hipschman | 2006-07-28 | [widl: Register types for coclasses.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9265d775849b0181fb3cd7efe244082128ca82a7) |
| Dan Hipschman | 2006-07-28 | [widl: Set typelib\_idx for coclasses when they're added to a typelib.](http://source.winehq.org/git/wine.git?a=commitdiff;h=90cdff9b3fbe0380cf38effb714376b26041359f) |
| James Hawkins | 2006-07-28 | [wininet: Only copy the relative filename into the UrlEntry structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c6040fccc2d8c8c9b3481f6ac0575e69ed3fbcd) |
| Dan Hipschman | 2006-07-28 | [widl: Encode coclass types in typelibs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=678ce9875f8e13c559caf457bccab6811a1cf082) |
| Thomas Kho | 2006-07-28 | [Maketest.rules.in: Fix comment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1afed1f8d8aaa46ec74e8f5cfa0b3c281ab92687) |
| Benjamin Arai | 2006-07-28 | [oleaut32: VarMonthName - Update error codes and helper functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0eed4603c506b1c0495b592489c5a4e6282ad0e1) |
| James Hawkins | 2006-07-28 | [msi: Add tests for MsiDatabaseImport.](http://source.winehq.org/git/wine.git?a=commitdiff;h=05bd17b8b7e27b555c4c6c21158da659aef08ca9) |
| James Hawkins | 2006-07-26 | [msi: Download the MSI package if it is a remote URL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d1617bea17b8614303ef5b19851e18f25b66a250) |
| James Hawkins | 2006-07-26 | [msi: Test the column types of MSI packages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=75c866ed58c5fcab66dc826249bb6f096bcb8608) |
| James Hawkins | 2006-07-26 | [msi: Test the states of a component with a compressed file.](http://source.winehq.org/git/wine.git?a=commitdiff;h=59a706bc2b60dcd74d528405194228d41383ed59) |
| James Hawkins | 2006-07-26 | [msi: Fix a typo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5842af1b951d5deb552130ea27da95e8f816a44e) |
| Thomas Kho | 2006-07-25 | [wcmd: Correct handling of quotes and /s flag when a command argument is present.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bff25ffe7991bde75904d34ca733f2178b088316) |
| James Hawkins | 2006-07-25 | [msi: Add tests for the WHERE SQL clause.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8144e171697bc3543c4c0b2ddd743ca3827db669) |
| Dan Hipschman | 2006-07-25 | [widl: Allow trailing commas in attribute lists.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b3632a1cd0e8c4633f00ac97325e583ebadaf60) |
| Dan Hipschman | 2006-07-24 | [widl: Fix redefinition of types in output.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f3d01fb07b38858c28156eb1ec1799765f65fd20) |
| Dan Kegel | 2006-07-24 | [winedos: Limit reported disk space to 1GB.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91f9746d2f8f564a508351490205b7c7a64b718e) |
| Dan Hipschman | 2006-07-24 | [widl: Support SAFEARRAY(type) syntax.](http://source.winehq.org/git/wine.git?a=commitdiff;h=12a9dfd62fcfb0be520b0bba2954b780dc994329) |
| James Hawkins | 2006-07-21 | [msi: Expand features with odd Display values.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e295bd97431fefdeac74f4c5c340c266bae1dd75) |
| James Hawkins | 2006-07-21 | [msi: Add tests for component and feature states.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dc0aad523ba7fa6fcb511ed9f080d3807b5b4cc8) |
| James Hawkins | 2006-07-21 | [msi: Don't display a feature if its Display value is zero.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf9886e6e0a4c6a862d88d26b8eaf7b6f9b8c6a5) |
| James Hawkins | 2006-07-21 | [msi: Set the component's initial state based on its attributes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cae3215a6fd78446fd356cb8720dd70adc734d69) |
| Benjamin Arai | 2006-07-21 | [oleaut32: Fix missing tests and heap errors for VarCat conformance.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b636e4dbf43c9054fb3ce66e674d1fdc8dd6be5b) |
| Dan Hipschman | 2006-07-21 | [widl: Allow write\_type to output full pointer types.](http://source.winehq.org/git/wine.git?a=commitdiff;h=82c11ce0025e386308623671f126646d0724051a) |
| Thomas Kho | 2006-07-21 | [server: Add new threads to end of thread\_list.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ff4ba394ed56b2ea94553f90ed7935e85669914) |
| Benjamin Arai | 2006-07-21 | [oleaut32: Fix temp variant initialization issues in VarCat.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4026a4c0a8d47f558ce1d303a9d8b92270e16474) |
| Benjamin Arai | 2006-07-20 | [oleaut32: Implements OLEFontImpl\_GetIDsOfNames.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f75b9f190f368956949277983a09757d3e5b1a67) |
| Benjamin Arai | 2006-07-20 | [oleaut32: OLEFontImpl\_GetIDsOfNames conformance test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31e3ad7150f5e308e5ead6f49fa0e87f7d2bafc4) |
| James Hawkins | 2006-07-19 | [msi: Implement the SetInstallLevel event.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ece0ae0a41b74f9ee37ad1dbe3835e82e997641c) |
| James Hawkins | 2006-07-19 | [msi: Forward MsiSetInstallLevel to an internal MSI\_SetInstallLevel that can be used ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=de73481c894ccea076fe53af5b743c77cfe7d1f5) |
| James Hawkins | 2006-07-19 | [msi: Rename SetFeatureStates to match the naming scheme of internal msi functions.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c7f0bb2c18b23003bd7c63cb9e8b9ab90cf9cec) |
| James Hawkins | 2006-07-19 | [msi: Update feature states after changing install levels, as they may have changed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7bcac31dcf4b37a0780efaf06540351e2c3543b3) |
| James Hawkins | 2006-07-18 | [msi: Add a stub implementation of MsiSourceListClearAll.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc56e92657ddb67c6374e51ae23b90207d44049b) |
| Benjamin Arai | 2006-07-18 | [oleaut32: Update error codes for VarMod.](http://source.winehq.org/git/wine.git?a=commitdiff;h=911af4dce9c0b0d5984491baae7e515647519d2e) |
| James Hawkins | 2006-07-18 | [msi: Sort SelectionTree items by their Display value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2396e2a59f822dd10975e82ed8224e1fe4b883c7) |
| Benjamin Arai | 2006-07-17 | [oleaut32: VarCmp - Corrected function description.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d42002b72c1218a8e46c3df2582ee05b4e8fe412) |
| Dan Hipschman | 2006-07-17 | [wpp: In recursive macro definitions, print the macro name instead of nothing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=804993deeababf0c80af65e8a95ab2ec4e4bce0a) |
| James Hawkins | 2006-07-17 | [msi: Update the feature components' states when a feature is selected.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7745a831a13adc0c8f55911009c3b2b57b8fa754) |
| Dan Hipschman | 2006-07-14 | [widl: Fix unterminated comment in generated code.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d68ec1d325e17b45194af58e455a567a79f45462) |
| James Hawkins | 2006-07-14 | [wininet: Add more tests for InternetCrackurl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1544731dbaf30c473be2ae254f2f24e3138babf) |
| James Hawkins | 2006-07-14 | [msi: Add handling for the ListBox dialog control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6de2ca845983dd93c3e9cdda97e8f6019b5f1f2f) |
| Dan Hipschman | 2006-07-14 | [widl: Support coclass forward declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2660b8f9c190890faf7f22054344e238f0b3edb5) |
| James Hawkins | 2006-07-13 | [shlwapi: Add tests for PathCommonPrefixA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c70bf5aaab747ca8966536d64c0047f1959001d6) |
| James Hawkins | 2006-07-13 | [shlwapi: Add tests for PathBuildRootA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a6f4ede2557d83c2f659b8f320e2b53658ac8448) |
| James Hawkins | 2006-07-13 | [msiexec: Also support options using a hyphen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8c3fc3a889bd6c5e0dc965d0aec4dad9fc5937db) |
| James Hawkins | 2006-07-13 | [msi: Add handling for the GroupBox dialog control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1adcf0087af491d2f1413d87ae225b17101568fc) |
| Dan Hipschman | 2006-07-12 | [gdi32: Add conformance test for GetTextExtentExPointW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fe3c9428c3975259e50eb2d87f60307fda154144) |
| Dan Hipschman | 2006-07-12 | [gdi32: Implement GetTextExtentPoint in terms of GetTextExtentExPoint](http://source.winehq.org/git/wine.git?a=commitdiff;h=f9047238134e1dbfd7eaedf81a6ee94788a4681d) |
| Thomas Kho | 2006-07-12 | [notepad: Change file not saved alert title to match Windows' notepad.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=724dd10ee80fe8b909c914dca07be13dacf251e0) |
| Thomas Kho | 2006-07-12 | [notepad: Change window title to be like Windows' notepad.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3ec165fd990d1d62bfa5dacb30d2592285c4917f) |
| James Hawkins | 2006-07-12 | [msi: Update the files target paths as well, because a parent directory might have ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=094915ae2c12f1b3122462890bcda20b8cb70f7c) |
| James Hawkins | 2006-07-11 | [urlmon: Implement URLDownloadToCacheFileW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e2bf4ff16449d4c90d2a9fb662dc0f506d7bcbbc) |
| Benjamin Arai | 2006-07-10 | [oleaut32: Conformance test and patch for VarCat.](http://source.winehq.org/git/wine.git?a=commitdiff;h=700adac9aca86a0aab85952ac0d4472a2e4dd842) |
| James Hawkins | 2006-07-10 | [msi: AppSearchReg shouldn't create the key it's looking for if it doesn't exist.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3b506c640866025eb791e806d756330cdb2b01d0) |
| James Hawkins | 2006-07-10 | [msi: Test how SetTargetPath affects the target paths of install files.](http://source.winehq.org/git/wine.git?a=commitdiff;h=15ad5de13c7046d65a1e7c9b6153dfc8e6dd7c62) |
| James Hawkins | 2006-07-08 | [advpack: Add tests for different configurations of INF filenames and](http://source.winehq.org/git/wine.git?a=commitdiff;h=ac9e421999a98598ba05e72a397f776d0c7bf698) |
| Thomas Kho | 2006-07-08 | [winex11: Use correct multiplier for negative relative mouse movements.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4598c973b22bb7d7bd4436866d29e86ef3e0644d) |
| James Hawkins | 2006-07-06 | [advapi32: Add tests for LookupAccountSid.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce58c3589ca98cfaeafb5f2b5e8902732483b315) |
| James Hawkins | 2006-07-06 | [advapi32: Get the token type in ImpersonateLoggedOnUser.](http://source.winehq.org/git/wine.git?a=commitdiff;h=409c6dc7b00a8ea6e1321d7f00b032bfe37711d7) |
| Thomas Kho | 2006-07-06 | [notepad: Change window classname from NPClass to Notepad.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0796fe256be7205ee336f2746c91daeb319938f3) |
| James Hawkins | 2006-07-03 | [wininet: Use a blank password if none is provided in FTP\_Connect.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8e96015ebb47c86625f70efac6b702122968636e) |
| James Hawkins | 2006-07-03 | [wininet: Error out if hInternet is a bad handle.](http://source.winehq.org/git/wine.git?a=commitdiff;h=545309c97fef6272b86563ca7bd7dbc856681038) |
| Thomas Kho | 2006-07-01 | [wcmd: Modify option parser to allow compound options.](http://source.winehq.org/git/wine.git?a=commitdiff;h=543716e1148bf67ca1e0130bf84cd77ff60ecd80) |
| James Hawkins | 2006-06-29 | [shlwapi: Add tests for PathCanonicalize.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b333f0c4d2babe40ab16a7a3f558266c94fd96b5) |
| James Hawkins | 2006-06-29 | [shlwapi: Add tests for PathFindExtensionA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad064915c957dd89e322bfe868c3b4c0d0c8e70a) |
| James Hawkins | 2006-06-27 | [msi: Read the font color from the database, and use it for the text control.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3c56550ea5141b48ec19a7a44b3e49f0bf7c6b2e) |
| James Hawkins | 2006-06-27 | [shlwapi: Add tests for PathAppendA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3a1a607a008f4ad1b5f1c3a248199fb2a12e277b) |
| James Hawkins | 2006-06-26 | [shdocvw: Upgrade the version to 5.50.4134.599.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e391387c9acc68ea84b8966f635d46be5d7b0134) |
| James Hawkins | 2006-06-26 | [setupapi: Fix SetupCloseInfFile when a NULL handle is given, with tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bce44161f1f836fbe53a6c2be6ca16478810f0d5) |
| James Hawkins | 2006-06-26 | [msiexec: Use CommandLineToArgvW instead of process\_args to reduce code duplication.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7c35db000b26852fc2bf4a7a7e349953f60d183f) |
| James Hawkins | 2006-06-26 | [shlwapi: Add tests for PathCombineA.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7412bddd363b22186d14e13e373bbf64cc116751) |
| James Hawkins | 2006-06-26 | [shlwapi: Add tests for PathAddBackslash.](http://source.winehq.org/git/wine.git?a=commitdiff;h=251d76888d70133d3afa2cb8c43a45420175d8c2) |
| James Hawkins | 2006-06-23 | [shell32: Add missing multiply by sizeof(WCHAR)l](http://source.winehq.org/git/wine.git?a=commitdiff;h=f921fa544aeb018286d49e58343f1c61ab4924fe) |
| James Hawkins | 2006-06-22 | [msi: Add tests for components that aren't associated with a feature.](http://source.winehq.org/git/wine.git?a=commitdiff;h=566beb788b75c3c94aa7d9d6c8601b468a5116ef) |
| James Hawkins | 2006-06-21 | [atl: Add a stub implementation of AtlModuleLoadTypeLib.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b865c07db978fc846484d895654bb2fac1051004) |
| James Hawkins | 2006-06-21 | [mapi32: Add a stub implementation of MAPIOpenLocalFormContainer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=092166696d05f0d1358a2153846d0377c7d98502) |
| James Hawkins | 2006-06-20 | [tools/wine.inf: Add d3d8.dll to the fake dlls list.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ce24c2a8a706cb016c2aaef7deb629e4ba7cca93) |
| James Hawkins | 2006-06-20 | [msi: Fix handling of the no-op identifier in the Directory table.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a1910e11bb4608469d2e70da7c00c651c0e12360) |
| James Hawkins | 2006-06-20 | [advpack: Implement DoInfInstall on top of the install framework.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a0208ef612708c7dd8e570760758d7da2405f9c) |
| James Hawkins | 2006-06-15 | [msi: Add tests for MsiInstallProduct.](http://source.winehq.org/git/wine.git?a=commitdiff;h=36bf71c17405c5efe469ebe8227e1f25c0e816ee) |
| James Hawkins | 2006-06-05 | [oleaut32: Only BYREF DispCallFunc args whose input args are not BYREF should be changed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=585763ffa91ba10291e2a2eff27b7dd8fd623611) |
| James Hawkins | 2006-06-05 | [oleaut32: Copy BYREF args directly if they have the same variant type.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e5bd51d28eaa3a7d72c583f7cd822218ca4b351) |
| Thomas Kho | 2006-04-28 | [user: Extend menu conformance test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bde9ca2b63a5e2d04bcd6a1c94d7bf04f4922d02) |
| Thomas Kho | 2006-04-27 | [user: Fix behavior when selecting disabled menu items.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8338605794c357eb7c1d319f3eec62a2efff3ea) |
| Thomas Kho | 2006-04-27 | [user: Allow menu WndProc to recognize VK\_[LR](http://source.winehq.org/git/wine.git?a=commitdiff;h=76104e1ccc2875dbb14331764913c07e75f3d0b7)MENU.] |
| Dan Kegel | 2006-04-22 | [msi: Fix missing case in MsiSourceListAddSourceEx.](http://source.winehq.org/git/wine.git?a=commitdiff;h=35f9a4797f52ae5e697c096015a9bafdd6a2c52e) |
| Thomas Kho | 2006-04-19 | [x11drv: Virtual key input scrubbing in X11DRV\_send\_keyboard\_input.](http://source.winehq.org/git/wine.git?a=commitdiff;h=75cd5e2101fb49ee9a7aca2f661d23604e7f619c) |
| Huw Davies | 2006-04-18 | [gdi32: Fix {Bit,Stretch}Blt fallbacks to StretchDIBits.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bf23ad0da7430afe69d2aff2a2b0549c05458db9) |
| Jacek Caban | 2006-04-14 | [shdocvw: Better window handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b81b614da824e54c80f7e32dcf2672519bbe20ce) |
| Jacek Caban | 2006-04-14 | [shell32: Don't crash in SHELL\_ExecuteW if psei-&gt;lpDirectory is NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=150bd5442cf6037f2760e42592190e62ea055edb) |
| Mike McCormack | 2006-04-13 | [wtypes.idl: Add size attribute to a void pointer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54d3060a2db33e160c144dd0bbd787c859ddd73a) |
| Mike McCormack | 2006-04-13 | [widl: Add support for VT\_I8 and VT\_UI8 to msft typelibs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1d453ab55139fe1481eb78640966ecd7fa3d73b3) |
| Aric Stewart | 2006-04-13 | [comctl32: Listview notify fix.](http://source.winehq.org/git/wine.git?a=commitdiff;h=097aec39ca86fb84cda58c1db0b84c2c035b1ef4) |
| Jacek Caban | 2006-04-12 | [shdocvw: Use GetClientRect, not GetWindowRect in create\_doc\_view\_hwnd.](http://source.winehq.org/git/wine.git?a=commitdiff;h=51bd5408d4b411924123bde72bae95fa9b00fa55) |
| Jacek Caban | 2006-04-12 | [shell32: Allocate wszApplicationName on the heap as it may be longer than MAX\_PATH.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b5125a79c4432b8d54f306418b175a51d6190ad) |
| Dmitry Timoshkov | 2006-04-12 | [avifil32: Avoid not necessary zeroing out of an allocated memory block.](http://source.winehq.org/git/wine.git?a=commitdiff;h=14aab5f3cb34cca8d24244622464eec39ae09a65) |
| Thomas Kho | 2006-04-12 | [x11drv: Properly handle VK\_LMENU input.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e81484c45863b4005023f0159661f746a4a3d50) |
| Mike McCormack | 2006-04-11 | [shdocvw: Move the private class factory declaration into factory.c.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c1caf43d10918f7f422b7c5ef4ea5d3c323da8d6) |
| Mike McCormack | 2006-04-11 | [avifil32: Fix a regression caused by patch removing GlobalAllocs by using HEAP\_ZERO ...](http://source.winehq.org/git/wine.git?a=commitdiff;h=aebc88d54bdc6d4a835d8a023aa1862114ee4d4d) |
| Mike McCormack | 2006-04-11 | [shdocvw: Register iexplore.exe as a COM local server.](http://source.winehq.org/git/wine.git?a=commitdiff;h=42c7372b6b8c64b8f6e9ea378c283d0903988bfd) |
| Jacek Caban | 2006-04-10 | [docobj.idl: Fix some enums declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc01e11eac8264799a18ae432e7b0d3264820b35) |
| Jacek Caban | 2006-04-10 | [exdisp.idl: Added SHDocVw type library declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91d7bb5211da89d80658159baad060c86b0129c3) |
| Jacek Caban | 2006-04-10 | [exdisp.idl: Added missing declarations.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5e99bd94f1a7251d68367d880e4e292d9f1b2cea) |
| Jacek Caban | 2006-04-10 | [exdisp.idl: Added missing attributes and fix some arguments names.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d5a380e9ef862b282df86140fe177451155c604) |
| Jacek Caban | 2006-04-10 | [exdisp.idl: Move declarations to better match to IE SDK.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d3cef6dc9bffea5aedf70f618ee90070f6f7226) |
| Dan Kegel | 2006-04-09 | [x11drv: Fix two clipboard bugs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d5292cb3f43c882d46e8a83475b047edec0ea633) |
| Jacek Caban | 2006-04-08 | [mshtml: Fix ref counting.](http://source.winehq.org/git/wine.git?a=commitdiff;h=417c10476041079a20143314de5c49bdf2e4dafe) |
| Alexandre Julliard | 2006-04-07 | [kernel: Fixed set\_process\_name for the winevdm case.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fcb771d9c0eafd812432b333cba6f2da0b4e5d8b) |
| Mike McCormack | 2006-04-07 | [shdocvw: Implement IEWinMain using a simple window frame.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d0873a74c314088426ea3e57fd2496c2d9fa78d) |
| Mike McCormack | 2006-04-06 | [shdocvw: Forward IWebBrowser2::Navigate calls to ::Navigate2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ba881a94d8ff29e20c9c8763a517001075a63bb8) |
| Alexandre Julliard | 2006-04-06 | [kernel: Show the exe name instead of wine-[kp](http://source.winehq.org/git/wine.git?a=commitdiff;h=9603ee07565d1ab8ae2f272094fcebab982933d9)thread in ps and top.] |
| Mike McCormack | 2006-04-05 | [shdocvw: Add class definition for InternetExplorer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=152541b94c48c03c528659835482ad30f48b09fb) |
| Mike McCormack | 2006-04-04 | [shdocvw: Stub implementation of IEWinMain.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fc33d3bca8fb2c87500ac4144d64c6621f7e3eca) |
| Mike McCormack | 2006-04-04 | [Add an implementation of iexplore.exe.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5a5b35cec791c7616595f04e67b73e44483a6a9e) |
| Dmitry Timoshkov | 2006-04-03 | [gdi: Move WineEngInit call before stock fonts creation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fd2ed6fffe495e243ce4480315f7bdb19d2a59e3) |
| Alexandre Julliard | 2006-03-31 | [loader: Hide the preloader from the ps output.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c20d6c409569a916231d14acd8a5a104cfedf74b) |
| Mike McCormack | 2006-03-30 | [WININET: Clean up HttpQueryInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae300883faa29ddad5c65aeac5cad682380e4cd3) |
| Mike McCormack | 2006-03-30 | [wininet: Clean up HTTP\_GetCustomHeaderIndex.](http://source.winehq.org/git/wine.git?a=commitdiff;h=92ddc1c851a01773221d3863dbad38a344630b0a) |
| Mike McCormack | 2006-03-30 | [wininet: Use a lookup table sorted by index so we don't need a loop to do lookups.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7f5e273214bb4d75824efc7133b366b4703450a6) |
| Mike McCormack | 2006-03-30 | [wininet: Make sure to set LastError when returning FALSE in HttpQueryInfo.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2571fa004a334818c1d9c0a438c974a9ce28106f) |
| Mike McCormack | 2006-03-28 | [server: Fix a race condition in the delivery of change notifications.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f5c1381e065bfab1903eebd7596f670b82c28509) |
| Alexandre Julliard | 2006-03-28 | [x11drv: Only warp the mouse pointer if it has actually moved.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bc15e1bc8195737e0f9ddc741cf4d9e79f500c55) |
| Alexandre Julliard | 2006-03-28 | [mshtml: Don't free the URL we have just stored in the callback object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=31332b3cd6d1c8fb0e11cbb2ff7d00a223468a8f) |
| Alexandre Julliard | 2006-03-27 | [server: Store window properties in the global atom table instead of](http://source.winehq.org/git/wine.git?a=commitdiff;h=641e9e382f8b8ae04296eb94673066e5e5566170) |
| Jacek Caban | 2006-03-27 | [mshtml: Added tooltip implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5f009f2540759d767f4fa696d855edfd21bc3dcd) |
| Mike McCormack | 2006-03-24 | [ntdll: Recursive notify is implemented.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23b74754fed40211550e5a6e224880a737107ad8) |
| Jacek Caban | 2006-03-23 | [mshtml: Added IHTMLElement2 implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ed10e5046c107971bd689b3c1564106d9ee6afce) |
| Jacek Caban | 2006-03-23 | [exdisp.idl: Added missing IE6 methods to DWebBrowserEvents2.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c2254468879430bb52aac5255c58ecf62a170b6) |
| Jacek Caban | 2006-03-22 | [mshtml: Clean up get\_all and tags (also fixes a typo).](http://source.winehq.org/git/wine.git?a=commitdiff;h=b88b981dcbb0b220ef1686a3acde2658c995c7fd) |
| Alexandre Julliard | 2006-03-22 | [server: New scheme for cleaning up objects on server exit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b00fb174f6b8ae8940f37c1229040a3cca84de74) |
| Alexandre Julliard | 2006-03-22 | [server: Class and global atoms should not be local to a window station.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9873494ced8405113381266b4d99c2a9f3002cb1) |
| Aric Stewart | 2006-03-22 | [twain: Add a property sheet UI for scanning.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8358c63e15b64f7e11a238e2b375121108148479) |
| Aric Stewart | 2006-03-22 | [twain: A few cleanups, using some consts from sane.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0bcc992162a5ce4a338c9210ef90e6a98dcf3254) |
| Alexandre Julliard | 2006-03-20 | [x11drv: Clear new bitmaps if they don't contain any data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ddc60c85f6747a96c93925b2fd785d1419f17dee) |
| Alexandre Julliard | 2006-03-20 | [configure: Use --rpath when linking dlls too.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1fd32cfa137867081f3a1ebf5a22b059e4c6dc83) |
| Alexandre Julliard | 2006-03-20 | [kernel: Avoid infinite waits in directory change tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=13c2f4742f776e40815287fce2d78cee1e8c265b) |
| Jacek Caban | 2006-03-18 | [mshtml: Optimize nsACString handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dbd582cf8423c2c3cb723386df37c89a59e45789) |
| Jacek Caban | 2006-03-18 | [mshtml: Better QueryInterface implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d9d3844860efc63590fa2df44605e543a9fa7bf) |
| Jacek Caban | 2006-03-18 | [mshtml.idl: Added more interfaces.](http://source.winehq.org/git/wine.git?a=commitdiff;h=144bb464c3089456fc19a1580dfa1898ccafb20c) |
| Alexandre Julliard | 2006-03-10 | [aclocal.m4: Avoid invalid characters in the cache variable name in WINE\_GET\_SONAME.](http://source.winehq.org/git/wine.git?a=commitdiff;h=30de3e8efe9211d6909a15610725cc8da5eeff70) |
| Alexandre Julliard | 2006-03-10 | [winefile: Refresh the drives and files upon WM\_DEVICECHANGE.](http://source.winehq.org/git/wine.git?a=commitdiff;h=04dad6218f64776712653ecdc24126a4d61f0d59) |
| Alexandre Julliard | 2006-03-09 | [user: Support packing/unpacking the WM\_DEVICECHANGE message.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a32b3e86ec3c6b83804d896ed1cc3438cd9dc482) |
| Jacek Caban | 2006-03-09 | [mshtml: Added beginning of getAttribute implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2c06b800b196887c287b6b2babb09edd989ec598) |
| Alexandre Julliard | 2006-03-09 | [dbt.h: Added DBTF\_ flags.](http://source.winehq.org/git/wine.git?a=commitdiff;h=18345170fd888ef54902bd8f80595bec3dc12f0c) |
| Jacek Caban | 2006-03-08 | [mshtml: Added IHTMLBodyElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=26b9c5e022f0ea05b903f7f3583c9ef2a6f64132) |
| Alexandre Julliard | 2006-03-07 | [explorer: Added desktop option.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a93b6a5945b2ffd29cc950fe8e8d6cd6cdf73261) |
| Jacek Caban | 2006-03-07 | [mshtml: Added get\_type, get\_value, get\_name and get\_checked](http://source.winehq.org/git/wine.git?a=commitdiff;h=92ff0e5019bbf6d052c496fb34b64e2e6976c7dd) |
| Jacek Caban | 2006-03-07 | [mshtml: Added get\_name and get\_value implementation of IHTMLTextAreaElement interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6fafc22930e6ecc8978ca249ccbff9335fdcfdce) |
| Alexandre Julliard | 2006-03-07 | [explorer: Merged systray support with the desktop window main loop.](http://source.winehq.org/git/wine.git?a=commitdiff;h=576e3b706299f21897fc09c15b767fd79e701e79) |
| Jacek Caban | 2006-03-07 | [mshtml: Added get\_name and get\_value implementation of IHTMLSelectElement interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4ac4246fd5435b02b042588bc1cbed4ef796bb9e) |
| Alexandre Julliard | 2006-03-07 | [server: Fixed length check in dump\_inline\_unicode\_string.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d531f1bb5b54c46eeedc794b29b4458a281d02a) |
| Alexandre Julliard | 2006-03-07 | [user: Launch explorer to manage the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1a4f6e579b6aab685fae2e649fd5accee7ec0b4f) |
| Alexandre Julliard | 2006-03-07 | [x11drv: Don't send an invalid WM\_NCCREATE to the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=116aaa169479a5e42aee6adcf3cf7b4d87beb18d) |
| Alexandre Julliard | 2006-03-06 | [server: Support for closing the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f978f615d8d89f5e3dc7056cfff7b34e1f174295) |
| Alexandre Julliard | 2006-03-06 | [user: Allow creating windows of the desktop class.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f874d20f54607dca0113e899c61af0bdaee9adba) |
| Alexandre Julliard | 2006-03-06 | [shell32: Fixed handling of null-terminated file list in SHFileOperation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b222001defc8d9db67232aae68f2d3a83c4ecd5d) |
| Alexandre Julliard | 2006-03-06 | [kernel: Better support for detached processes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a401f3c4bb5819e6fcfefa9587eca60796531c4a) |
| Jacek Caban | 2006-03-06 | [mshtml: Added IHTMLTextAreaElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f897239c46dabeeeb06827f53463e651ee70648) |
| Alexandre Julliard | 2006-03-06 | [server: Added unlink\_named\_object function.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8cea993033944e927e6bcbceda647322d00916e5) |
| Jacek Caban | 2006-03-06 | [mshtml: Added IHTMLInputElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b3eab6e35cf038330880426d0dd2e324db6721f) |
| Jacek Caban | 2006-03-06 | [shdocvw: Added get\_LocationURL implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=87e04f2f4a020a4209f051c2ee39f4c0a463d985) |
| Alexandre Julliard | 2006-03-06 | [server: Avoid crash in set\_thread\_desktop if the thread doesn't have a queue.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71b94726d9661d2f51afe4bd72539de656dcd0a3) |
| Alexandre Julliard | 2006-03-06 | [user: Allow some Wine internal messages to act on the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=70d42f9d43dbadfdc1692ef574acc7e9b8ee01f2) |
| Alexandre Julliard | 2006-03-06 | [x11drv: Make sure to never manipulate the root window, even if we own](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d5f5447eaae4837d8da9210d21fd3265a0073d7) |
| Jacek Caban | 2006-03-06 | [mshtml: Added IHTMLSelectElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54cce2e7ceccbea268718ea51aea98bac7997627) |
| Alexandre Julliard | 2006-03-06 | [server: Return real parent and owner in the create\_window request.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4be3d4c12b916d2f17c22f09bcf087f7b8ce7390) |
| Jacek Caban | 2006-03-06 | [mshtml: Added IHTMLElementCollection::tags implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3d6859935599321270d6c18a12e3767044963e54) |
| Alexandre Julliard | 2006-03-06 | [libwine: Export a function to retrieve the data directory (based on a](http://source.winehq.org/git/wine.git?a=commitdiff;h=2f026d1694d6e34b6e2d9d4d61ef5632e6f3251d) |
| Alexandre Julliard | 2006-03-06 | [server: Infrastructure for having a thread own the desktop window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=251be542aca1dbf418e5c15e4adb0c5a2d7d3fc0) |
| Alexandre Julliard | 2006-03-06 | [shell32: Store only the file attributes in the file list for SHFileOperation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=23cb632be2265cf9f927cae54237c78dea161358) |
| Alexandre Julliard | 2006-03-06 | [mlang: Decrement the module refcount when an object is destroyed.](http://source.winehq.org/git/wine.git?a=commitdiff;h=19a3adb9580ccf32c66c0ff4864a68d31044684f) |
| Alexandre Julliard | 2006-03-06 | [shell32: Grow the file list dynamically in SHFileOperation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1110d62752947c82723d1eb252be8e49cac3dfb0) |
| Jacek Caban | 2006-03-05 | [mshtml: Added more interfaces to mshtml.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ee1e7e503fb641b4bb21c2561111ca081f7e1475) |
| Jacek Caban | 2006-03-05 | [mshtml: Added IHTMLElementCollection implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d6d76870cb1ccb83f6feb8736dfca6d9dc1d984d) |
| Jacek Caban | 2006-03-05 | [mshtml: Added IHTMLElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=874fd57841f8d9670c50429b8b28d6b3627b0bb3) |
| Jacek Caban | 2006-03-05 | [shdocvw: Beginning ShowContextMenu implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a3a554c9b4aa3a894864a7c3f3eef6bac053eb6) |
| Jacek Caban | 2006-03-05 | [mshtml: Added get\_documentElement implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6ef5f9556215ac4b3426028cc7156eaa133d20ef) |
| Jacek Caban | 2006-03-05 | [mshtml: Added IHTMLDOMNode implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54036bf6efa06337f5d8649037246f6a75ec652d) |
| Dmitry Timoshkov | 2006-03-04 | [winebrowser: Use CP\_UNIXCP when translating URL passed on command line](http://source.winehq.org/git/wine.git?a=commitdiff;h=182a66c0db3a9fa45c032f82f45ff155e3120ff5) |
| Aric Stewart | 2006-03-03 | [shell32: Skip dot directories in SHFileOperation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c29b7c352438669ee22961466360e926a831d313) |
| Huw Davies | 2006-03-02 | [gdi: Better support for 1bpp dib sections.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b55746ab62739fc1e4c0d4a15484e0e8337bab75) |
| Jacek Caban | 2006-03-01 | [mshtml: Beginning support for links opened in a new frame.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d656f996f118667a9a455c08a950d4f4ab647a0b) |
| Jacek Caban | 2006-03-01 | [shdocvw: Don't call hlink\_navigate if HLNF\_OPENINNEWWINDOW is set.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d3a5921e8eeaab5f33bb074c77bb04d8ccd0fa0a) |
| Jacek Caban | 2006-03-01 | [mshtml: Use NSContainer as 'This' of its window.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2be7ffdf594594f74a702ebc67a8bf4746bf6bd3) |
| Alexandre Julliard | 2006-02-28 | [wrc: Integer ids can be used for control labels instead of strings.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8f08fe6c0dc9ad3f2d5e00f2b79488eba622cd26) |
| Dmitry Timoshkov | 2006-02-28 | [notepad: Wrap long lines by default like Windows does.](http://source.winehq.org/git/wine.git?a=commitdiff;h=832ec7056511ee04dc3d4fdce09acf2ceb2c58dd) |
| Mike McCormack | 2006-02-28 | [server: Print a message if wineserver crashes and we don't dump cores.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0cd0626de019c8ca288ed8a61a053c0f485c5c5c) |
| Jacek Caban | 2006-02-27 | [mshtml: Added nsIInterfaceRequestor implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=91369e20e756313f586de03da1354b4f621985fe) |
| Jacek Caban | 2006-02-24 | [mshtml: Return error in NewChannelFromURL if retval is NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b7e8057eecc14d38d41b9b28cb52c77557655330) |
| Jacek Caban | 2006-02-24 | [mshtml: Improve ConfirmEx hack.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a611b20c2621d4fccfa2b07d4ee357035b10e8db) |
| Jacek Caban | 2006-02-24 | [mshtml: Added nsIURI::Clone implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9b6c08a243c374bdd6dd58fcec5d6e72b2300bb9) |
| Jacek Caban | 2006-02-24 | [mshtml: Don't add null byte to post data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=71b881e4ba75bd2cccde863e55cdd4189d946c35) |
| Jacek Caban | 2006-02-24 | [mshtml: Init nsIOService as soon as possible.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4f9c9a16ad24af79a0de60053290bc210c1f3e00) |
| Dmitry Timoshkov | 2006-02-23 | [gdi: Use &quot;MS Sans Serif&quot; as default sans serif font, not Arial.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69a23a608eea59624b2f37ab424e0f42b3da5baf) |
| Huw Davies | 2006-02-23 | [gdi32: Fallback to StretchDIBits if the driver doesn't support BitBlt.](http://source.winehq.org/git/wine.git?a=commitdiff;h=66a05b2aec118946d75f159237a3c73df38f2486) |
| Mike McCormack | 2006-02-22 | [server: Add directories to recursive watches as they're opened.](http://source.winehq.org/git/wine.git?a=commitdiff;h=42121085985b3995692c4b40ee1b127963785223) |
| Mike McCormack | 2006-02-22 | [server: Make sure we don't get into an infinite loop freeing inodes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=309a9bf36fa114ad59b61987cf27b4f39faf7125) |
| Mike McCormack | 2006-02-21 | [kernel32: Add a short test for GetOverlappedResult.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f4b447aee7546c9921dd3a9c8d81ccdc6b1b1fae) |
| Mike McCormack | 2006-02-21 | [server: Track created and removed directories in the tree of inodes for inotify.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e4faabfa64aa0c89db482fc780ed1a7f51efa53e) |
| Aric Stewart | 2006-02-21 | [twain: Implment DG\_IMAGE/DAT\_IMAGEMEMXFER/MSG\_GET.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6976e2016d28249988ed975657f704fb5682b715) |
| Mike McCormack | 2006-02-21 | [kernel32: Add a simple test for recursive notification.](http://source.winehq.org/git/wine.git?a=commitdiff;h=54dfdb9b006fcd310a73d1e6bdf388cecd6c13d1) |
| Alexandre Julliard | 2006-02-21 | [server: Avoid hang on process startup.](http://source.winehq.org/git/wine.git?a=commitdiff;h=492661079c01313ad46797c984a09a2010d3ebe5) |
| Alexandre Julliard | 2006-02-21 | [shell32: Use more reasonable timeouts in shlexec test.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39a1a9422149a0d3d081f02d540423eac131bfaa) |
| Jacek Caban | 2006-02-21 | [shdocvw: Added correct implementation of IProvideClassInfo::GetGUID.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0c12e2663b6964d1cfc44b5546800e42452aba3b) |
| Mike McCormack | 2006-02-20 | [server: Distinguish between a directory and a file changing in](http://source.winehq.org/git/wine.git?a=commitdiff;h=a2813f7c2ef879fee94948eb4f935448e2f48152) |
| Jacek Caban | 2006-02-20 | [mshtml: Create nsIChannel for protocols not handled by Gecko.](http://source.winehq.org/git/wine.git?a=commitdiff;h=746616903481155b576c201ed734ebe9a61a82a7) |
| Alexandre Julliard | 2006-02-20 | [configure: Use --rpath if supported when building binaries to point to](http://source.winehq.org/git/wine.git?a=commitdiff;h=5ed59015b290c7c1238c7d08cacc299f0aa151e2) |
| Jacek Caban | 2006-02-20 | [mshtml: Set default original uri in NewChannelFromURI.](http://source.winehq.org/git/wine.git?a=commitdiff;h=416f504cdd340b8f75ea396245e7c1dad6499cbb) |
| Jacek Caban | 2006-02-20 | [shdocvw: Change FIXMEs to TRACE in IDispatch's methods as they return](http://source.winehq.org/git/wine.git?a=commitdiff;h=00f249022cdc6ae6ec04be17dfafecb38c34ab74) |
| Mike McCormack | 2006-02-17 | [server: Use a single inotify watch, as it scales better with a large](http://source.winehq.org/git/wine.git?a=commitdiff;h=fbc00db3f6cc2cf2434aa7063039df95329c64f2) |
| Alexandre Julliard | 2006-02-17 | [libwine: Set the default bindir and dlldir from argv0 if dladdr is not available.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e95a2c2111add8d40d486846fae844715577ef56) |
| Alexandre Julliard | 2006-02-17 | [ntdll: Remove no longer used oldcwd in start\_server.](http://source.winehq.org/git/wine.git?a=commitdiff;h=dcdb0d0b34a4f4d545bd307d0ff041eec3555220) |
| Jacek Caban | 2006-02-17 | [mshtml: Fix post data parsing.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d2389dc0cf16511266884df583f5d86fd5357cf0) |
| Alexandre Julliard | 2006-02-17 | [libwine: Compute relative paths for bin and dll directories at compile time.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b5e11c341c11b3a417d5845d8ff11aca77b339d) |
| Alexandre Julliard | 2006-02-17 | [tools: Added 'relpath' tool to compute relative Unix paths.](http://source.winehq.org/git/wine.git?a=commitdiff;h=35842ca71763682dbae233115a1ab7004bf8cf8d) |
| Alexandre Julliard | 2006-02-17 | [libwine: Add the runtime library path to the front of the dll paths list.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1269f43c5a68e03b526098fb18dd0edd42858ceb) |
| Alexandre Julliard | 2006-02-16 | [libwine: Only use the library directory if it's an absolute path.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ca6fd0d4eceae51f816457f425111a811d6ef057) |
| Thomas Kho | 2006-02-16 | [riched20: Implement EM\_SCROLLCARET and EM\_GETSCROLLPOS.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bfb3c756eb5f956904e5f3154eb09be34aa63e94) |
| Alexandre Julliard | 2006-02-16 | [libwine: Try the current load path in priority before the](http://source.winehq.org/git/wine.git?a=commitdiff;h=9dffd134ddcab7d87f2507e3bc37a8ee8029f5dc) |
| Juan Lang | 2006-02-16 | [wininet: Use CertNameToStr for INTERNET\_OPTION\_SECURITY\_CERTIFICATE\_STRUCT](http://source.winehq.org/git/wine.git?a=commitdiff;h=89529f8a8ebcdf63fb176e853a59158cbdf39da4) |
| Jacek Caban | 2006-02-16 | [shdocvw: Unaccess post data only if we've accessed it before.](http://source.winehq.org/git/wine.git?a=commitdiff;h=76a361af8215fa8f8be741c14afad84ae3f1770f) |
| Alexandre Julliard | 2006-02-16 | [libwine: Don't rely on argv[0](http://source.winehq.org/git/wine.git?a=commitdiff;h=767ad69a456f4ba2e35d297069188a0e5773a62c) in wine\_exec\_wine\_binary if we can get] |
| Jacek Caban | 2006-02-15 | [shdocvw: Added beginning IHlinkFrame::Navigate implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f98843e8cc5b165dbc724bf8213e2827ad65ca94) |
| Jacek Caban | 2006-02-15 | [shdocvw: Added client site's IServiceProvider interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ad5d88c67a7999ef380e48e5ea1011217e192a0a) |
| Jacek Caban | 2006-02-15 | [mshtml: Added hack to allow pass post data to IPersistMoniker::Load.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4b511edf8d5ab2a0ab0fe08d762ec2ded445bcd0) |
| Jacek Caban | 2006-02-15 | [mshtml: Added ref counting to NSContainer.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4acea60922128283e2b10f2e202fb428206b3abc) |
| Jacek Caban | 2006-02-15 | [shdocvw: Navigate2 rewrite.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0dbbd90c6a8346569316fc00b07d4817556167d4) |
| Juan Lang | 2006-02-15 | [crypt32: Output string type in trace.](http://source.winehq.org/git/wine.git?a=commitdiff;h=09b6cf971ff1de7574dcb7c18d297cab34bb7922) |
| Thomas Kho | 2006-02-15 | [riched20: Extend EM\_FINDTEXT conformance tests and fix 2 problems they expose.](http://source.winehq.org/git/wine.git?a=commitdiff;h=087af502ea547d4fa804bca688e00cb351ed13f7) |
| Dmitry Timoshkov | 2006-02-14 | [winmm: Protect drivers list by a critical section.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f29d4af34b4ef88838d545788de0d5f107ff6375) |
| Dmitry Timoshkov | 2006-02-14 | [msvfw32: Disable datarate, keyframe and quality controls to not](http://source.winehq.org/git/wine.git?a=commitdiff;h=f1e120ba7ea514fbf8c916e7608f9f165fb84135) |
| Jeremy White | 2006-02-14 | [twain: Reconcile sane's long names to TWAIN's 32 byte limit.](http://source.winehq.org/git/wine.git?a=commitdiff;h=63e8d34a42f717897635fa1d6bc39fb805bc1ff2) |
| Dmitry Timoshkov | 2006-02-14 | [msvfw32: Initialize lpbiIn member of the COMPVARS structure.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5de3d7df3266f7888be7164f29654dc80511ee24) |
| Jeremy White | 2006-02-14 | [twain: Make structures respect 2 byte packing requirements.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5b04c3ea5aaf514a66bf5d06a606b3ec2b9ac1e7) |
| Dmitry Timoshkov | 2006-02-13 | [msvfw32: Fix typos in the control state handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d4774ba1c66e9f4acabf977ecfb1d763e30eaa1f) |
| Jacek Caban | 2006-02-13 | [mshtml: Handle IHlinkFrame service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cb880d7cc70f48804e052a3cd45d1e7804daa951) |
| Dmitry Timoshkov | 2006-02-11 | [msvcrt: localtime should accept any positive time value.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea0e7b339751c16dca08c73cfc292a843f641bda) |
| Thomas Kho | 2006-02-11 | [riched20: Fixed bounds error when finding text forward.](http://source.winehq.org/git/wine.git?a=commitdiff;h=caffa53227d37f35bc32c03733dfc94556ff513f) |
| Dmitry Timoshkov | 2006-02-11 | [msvfw32: Call codec's Configure dialog if the codec supports it.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cad998112ece02f9a768083462c60832f1cfcbb6) |
| Dmitry Timoshkov | 2006-02-11 | [Handle ICM\_CONFIGURE request in ICCVID and MSVIDC32 codecs.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b4b3e6a165723b965af7b8352932ddf91fc404e8) |
| Thomas Kho | 2006-02-11 | [riched20: Added tests for EM\_FINDTEXT and EM\_FINDTEXTEX messages.](http://source.winehq.org/git/wine.git?a=commitdiff;h=482ab27e8d3cf6414d4db7c940328d07e14776f4) |
| Alexandre Julliard | 2006-02-11 | [configure: Added a WINE\_CHECK\_LIB\_FUNCS macro to check for functions](http://source.winehq.org/git/wine.git?a=commitdiff;h=2d1a6274ee8c8fc8ac33f5ed53892711492321db) |
| Alexandre Julliard | 2006-02-11 | [configure: Added check for dladdr in libdl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=266c609dd1dab8caab71ea1cc3949dacfcde8c40) |
| Alexandre Julliard | 2006-02-11 | [libwine: Use dladdr if supported to get the run-time path of libwine.so](http://source.winehq.org/git/wine.git?a=commitdiff;h=0b34fb365657b9983a591610b2d80e298623d6f0) |
| Aric Stewart | 2006-02-10 | [ntdll: gcc 2.95 compile fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d7187d79bdaa616332b33ef4acb3d8144e2dc9f8) |
| Jacek Caban | 2006-02-10 | [mshtml: Added nsIUploadStream implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=af6395774c10b4e7932e3044af5ce9dbf380b046) |
| Jacek Caban | 2006-02-10 | [mshtml: Added more defines to mshtmlhst.idl.](http://source.winehq.org/git/wine.git?a=commitdiff;h=adb1335e4e458968dbce03e087c66d51783e91cf) |
| Jacek Caban | 2006-02-10 | [mshtml: Added test of IHlinkFrame service.](http://source.winehq.org/git/wine.git?a=commitdiff;h=4a34d8e6424a5174ab52c657fc9ab5d8c8995465) |
| Jacek Caban | 2006-02-09 | [mshtml: Added wrapper of nsIChannel.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ae23f8d8cbac12d984394bfd446b0118ecdb29fd) |
| Jacek Caban | 2006-02-09 | [mshtml: Get rid of HTMLDocument\_OnLoad and move its job to AsyncOpen.](http://source.winehq.org/git/wine.git?a=commitdiff;h=990e20c9922d4b058242f4eb7b9da845af8d38de) |
| Aric Stewart | 2006-02-09 | [advapi32: Fix for RegNotifyChangeKeyValue.](http://source.winehq.org/git/wine.git?a=commitdiff;h=910806393dbffc77094652cb7dfff93217e3e4eb) |
| Jacek Caban | 2006-02-09 | [mshtml: Added wrapper of nsIOService.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8aeb04934122dd0d4878a537ea0bf3da481515a1) |
| Jacek Caban | 2006-02-09 | [mshtml: Better ns\*String handling.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7080c8d98ebc46fef3bedcb457e0be4643616a3d) |
| Juan Lang | 2006-02-09 | [crypt32: Fix up decoding.](http://source.winehq.org/git/wine.git?a=commitdiff;h=69698f9b44ce78b6e60e91e9664779e8a0e5383b) |
| Dmitry Timoshkov | 2006-02-09 | [regsvr32: Call OleInitialize before registering a DLL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2c59936fee254cfae4c646fccb3a6cc3f3c92f27) |
| Jacek Caban | 2006-02-09 | [mshtml: Added wrapper of nsIURI interface.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1b31475fdb2b9a46b557225d319a93671d895458) |
| Juan Lang | 2006-02-09 | [crypt32: Fix a fixme, and remove an old comment.](http://source.winehq.org/git/wine.git?a=commitdiff;h=02c4956157033896077b4027834f11f8dcdb56f3) |
| Jacek Caban | 2006-02-08 | [shdocvw: Remove IQuickActivate interface implementation that is not](http://source.winehq.org/git/wine.git?a=commitdiff;h=fa31cfb0b31c19839bd13b05a9d2d2e7a6b9b3b7) |
| Alexandre Julliard | 2006-02-08 | [server: Fixed handling of inotify record length.](http://source.winehq.org/git/wine.git?a=commitdiff;h=e979832dda71deeea092c31046f543fbeec13c5c) |
| Jacek Caban | 2006-02-08 | [shdocvw: Includes clean up.](http://source.winehq.org/git/wine.git?a=commitdiff;h=5d854158b8c9d67968802a3b27bd8407dce2b28c) |
| Jacek Caban | 2006-02-08 | [shdocvw: Added IHlinkFrame stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=461a0102c53e0d5704d5a0d949a90f70841cc1fd) |
| Jacek Caban | 2006-02-08 | [urlmon.idl: Added BINDINFOF declaration.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e3be46855c44fe4d2dbde42c0cca53be9b2d8c4) |
| Mike McCormack | 2006-02-07 | [kernel32: More test cases for ReadDirectoryChangesW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=7a61f086f17057a19ad3a65e2f177bbe3de136ac) |
| Dmitry Timoshkov | 2006-02-07 | [msvideo: Add a codec to the compressors list only if it supports](http://source.winehq.org/git/wine.git?a=commitdiff;h=75c436246d7eaf3d268a30e7401d289e6dd6e399) |
| Dmitry Timoshkov | 2006-02-07 | [x11drv: Copy the whole image at once if appropriate.](http://source.winehq.org/git/wine.git?a=commitdiff;h=729eaa6920a672acc0d8b682bcc9336b8575a364) |
| Dmitry Timoshkov | 2006-02-07 | [Clearly indicate that ICCVID and MSVIDC32 do not support compression.](http://source.winehq.org/git/wine.git?a=commitdiff;h=538ed06c41521fa8f884ecf39a7e617fafb43bc1) |
| Mike McCormack | 2006-02-07 | [kernel32: ReadDirectoryChangesW fixes.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0790f955897d5664997d7263fbd3e42165eda548) |
| Mike McCormack | 2006-02-06 | [ntdll: Add some more tests for NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bad5f92f540da2e7da9d1dad77a12b6a3e860b35) |
| Mike McCormack | 2006-02-06 | [server: Fill in NtNotifyChangeDirectoryFile's buffer with change data.](http://source.winehq.org/git/wine.git?a=commitdiff;h=01932119464a2a97421daeee1cdd8200646a67a1) |
| Alexandre Julliard | 2006-02-05 | [server: Fixed compile without inotify.](http://source.winehq.org/git/wine.git?a=commitdiff;h=cf9ced5e691ccaf76bc87f5171239fd5fe838d85) |
| Dmitry Timoshkov | 2006-02-04 | [msvfw32: Do not overwrite fccType in the codec enumeration proc.](http://source.winehq.org/git/wine.git?a=commitdiff;h=3f2e9681a60f87a5489bc5d5595f9a6496b5e013) |
| Dmitry Timoshkov | 2006-02-03 | [wine.inf: Change fcc type of builtin video codecs in system.ini to be](http://source.winehq.org/git/wine.git?a=commitdiff;h=de60d1e3bc616db9cb02b65346ecfcd592b659a7) |
| Dmitry Timoshkov | 2006-02-03 | [Add support for CDM\_HIDECONTROL message in the file open dialog.](http://source.winehq.org/git/wine.git?a=commitdiff;h=c8c8f1b8badf601bc4f9c8551573b5ca9b7f9540) |
| Dmitry Timoshkov | 2006-02-03 | [Add a check for icinfo-&gt;fccType in DRV\_OPEN message handler of builtin](http://source.winehq.org/git/wine.git?a=commitdiff;h=c13ae562892841a680ee68d965c8deadc47c15b2) |
| Mike McCormack | 2006-02-03 | [ntdll: Add FILE\_ACTION and FILE\_NOTIFY\_CHANGE\_ defines for streams.](http://source.winehq.org/git/wine.git?a=commitdiff;h=39f711ae6ec107c4a12ac900df574e79c161873b) |
| Alexandre Julliard | 2006-02-03 | [wine.inf: Make FourCC codes uppercase again until we can figure out](http://source.winehq.org/git/wine.git?a=commitdiff;h=19b89289ee077f7cc56148f05c6aff4549af234b) |
| Juan Lang | 2006-02-02 | [crypt32: Implement CertRDNValueToStrW and CertNameToStrW, with tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ede2e24a6af7677217486cc2f213dfebac15314a) |
| Mike McCormack | 2006-02-02 | [kernel32: FindFirstChangeNotification needs a static IO\_STATUS\_BLOCK.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d77baf358b2ba376d68ed9f590fe1d413e9f12c9) |
| Dmitry Timoshkov | 2006-02-01 | [wine.inf: Remove %1 from [http|htmlfile](http://source.winehq.org/git/wine.git?a=commitdiff;h=f03c86a27387cd1dc27c371d52a7c72d83b70481)\shell\open\command.] |
| Juan Lang | 2006-02-01 | [crypt32: Implement CertRDNValueToStrA and CertNameToStrA, with tests.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6a3b3f8635669ddf6fdae8d2d6a1b7c1a9ab3771) |
| Mike McCormack | 2006-01-31 | [kernel: Add some test cases for ReadDirectoryChangesW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9e2b6687f6ec1bbda1af684571ea9a7a9b7c6223) |
| Alexandre Julliard | 2006-01-31 | [kernel: Set the overlapped structure status in ReadDirectoryChanges.](http://source.winehq.org/git/wine.git?a=commitdiff;h=096000df90fbd047bd7893fbd344572514167d9b) |
| Mike McCormack | 2006-01-30 | [server: Initial inotify support.](http://source.winehq.org/git/wine.git?a=commitdiff;h=fdf0c684f56d8d679def550b92875fcddd219d9e) |
| Mike McCormack | 2006-01-30 | [kernel: Add some more tests for FindFirstChangeNotification.](http://source.winehq.org/git/wine.git?a=commitdiff;h=bd185ff3de84edf0ff38bb1ba18d34a1b9969b8c) |
| Alexandre Julliard | 2006-01-30 | [Fixed creation of PS\_ALTERNATE pens.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6b76244bf42a82f523f1c6c22607187dc1ce9c7d) |
| Alexandre Julliard | 2006-01-27 | [shell32: Fixed a couple of FindFirstFile handle leaks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d37a119ee66ad43099791605a748013ec69c7e2f) |
| Alexandre Julliard | 2006-01-27 | [server: Make the FILE\_SHARE\_DELETE sharing checks depend on DELETE](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b0feb253bc569a39e724a8da006735166fc1b32) |
| Mike McCormack | 2006-01-27 | [kernel: Partially implement ReadDirectoryChangesW using NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=700575955782bed874734610476aab6c8826f775) |
| Alexandre Julliard | 2006-01-27 | [server: Fixed low-level hardware hooks.](http://source.winehq.org/git/wine.git?a=commitdiff;h=6d85f3bf218faa25012d7d2f5b1c2aaa52f67631) |
| Mike McCormack | 2006-01-27 | [kernel32: Implement FindFirstChangeNotification with NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53dab1520055b089f1b40d3164245b7890843294) |
| Mike McCormack | 2006-01-27 | [server: Fix the file notification interface to use directory handles.](http://source.winehq.org/git/wine.git?a=commitdiff;h=08351071fd304748c86de4d6285f7ef5b8f0bd17) |
| Jacek Caban | 2006-01-26 | [shdocvw: Added client site's IOleCommandTarget stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=254bdf08f147720d8d5305423652b7cf5f7d7624) |
| Jacek Caban | 2006-01-26 | [shdocvw: Added WebBrowser's IOleCommandTarget stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=1b966122f85817195f3d32c1cf03d33e7f6abafb) |
| Jacek Caban | 2006-01-26 | [shdocvw: Added client site's IDispatch stub implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e1ef8ac2ef68faee2d35ff8a4e3dc6dbd054899) |
| Alexandre Julliard | 2006-01-25 | [wine.inf: Don't overwrite registry keys that users may want to change.](http://source.winehq.org/git/wine.git?a=commitdiff;h=f8f34d9fabb2be7582158fc74548f092dc2682f3) |
| Jacek Caban | 2006-01-25 | [shdocvw: Store IDocHostUIHandler interface in the WebBrowser object.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9cbe52b111b774c3482973b7fc1363c875c15501) |
| Jacek Caban | 2006-01-25 | [shdocvw: Added TranslateUrl implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=53c469f1e869ff07e80240cf8fb104eebeb10558) |
| Alexandre Julliard | 2006-01-25 | [x11drv: Always set GC function to GXcopy for the BitBlt DIB optimization.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0e08584462afd57c95af2cd4a5afa5a824975a66) |
| Jacek Caban | 2006-01-24 | [Added mshtmcid.h.](http://source.winehq.org/git/wine.git?a=commitdiff;h=ea6e5b969a255733fefc4e37eeaf6a39245ab7e4) |
| Alexandre Julliard | 2006-01-24 | [server: Use the new set\_fd\_user function in create\_serial().](http://source.winehq.org/git/wine.git?a=commitdiff;h=ab5ca5c04829642fbf1cff1a6c530e6fe1afd313) |
| Mike McCormack | 2006-01-24 | [server: Modify open\_fd to create an fd without a user.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9a7124e8159dc9ff3bcb3b04b970264ca77c1a47) |
| Dmitry Timoshkov | 2006-01-23 | [ICCompressorChoose should initialize fccType and fccHandler fields](http://source.winehq.org/git/wine.git?a=commitdiff;h=2a93c2f23defc6a4aec7a7335a5a792dd808011f) |
| Mike McCormack | 2006-01-23 | [ntdll: Forward ZwNotifyChangeDirectoryFile to NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2735fc58b990a94554e62cd8287fcd63962b65a9) |
| Aric Stewart | 2006-01-20 | [wininet: INTERNET\_OPTION\_SECURITY\_CERTIFICATE\_STRUCT work.](http://source.winehq.org/git/wine.git?a=commitdiff;h=8b0883576ee7c691cc57d68af6f5050fea981827) |
| Jacek Caban | 2006-01-20 | [shdocvw: Added GetWindow implementation.](http://source.winehq.org/git/wine.git?a=commitdiff;h=360a4aff2982a7d34595f25cd2f9f3f7a4caa4d7) |
| Aric Stewart | 2006-01-19 | [shell32: Update shellpaths My Pictures, My Video, My Music to be under](http://source.winehq.org/git/wine.git?a=commitdiff;h=265c8a5d7329a1512db900a799bd66013365b295) |
| Jacek Caban | 2006-01-18 | [shdocvw: Deactivate document in SetClientSite if ClientSite is NULL.](http://source.winehq.org/git/wine.git?a=commitdiff;h=47f796c6293c8a174006b2ab6de1316c407ab29e) |
| Mike McCormack | 2006-01-17 | [ntdll: Use FILE\_OPEN instead of OPEN\_EXISTING when calling NtCreateFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=9c58884161729aae445e25e15c28b87837f5cbff) |
| Mike McCormack | 2006-01-17 | [ntdll: Add a test for NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=2e32a425db6bcb86804517761686f31169ff3b80) |
| Mike McCormack | 2006-01-17 | [server: Make sure to release the fd we grabbed in all cases.](http://source.winehq.org/git/wine.git?a=commitdiff;h=213e01e606bc0434059fced84b2bcf349e622bcc) |
| Mike McCormack | 2006-01-16 | [kernel32: Add FILE\_NOTIFY\_INFORMATION.](http://source.winehq.org/git/wine.git?a=commitdiff;h=b8e5e0168a70432e6991289643254074b103b42b) |
| Mike McCormack | 2006-01-16 | [ntdll: Use the NTAPI definition of EXCEPTION\_ACCESS\_VIOLATION.](http://source.winehq.org/git/wine.git?a=commitdiff;h=a3348cf4a0179a4d2097d59c27096d5f9d250fe9) |
| Mike McCormack | 2006-01-16 | [ntdll: Add a stub implementation of NtNotifyChangeDirectoryFile.](http://source.winehq.org/git/wine.git?a=commitdiff;h=0c728255a4f0188acf379aa750437b6c3cd11d87) |
| Jacek Caban | 2006-01-14 | [mshtml: Better handling of IDocHostUIHandler in SetClientSite.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d44364d3fe61dca9d7d3f1189e8d24fcbae2336d) |
| Aric Stewart | 2006-01-14 | [explorer: Handle /select arguments correctly with the new winefile](http://source.winehq.org/git/wine.git?a=commitdiff;h=7439c29d07f7259e789f1d6c54c2feb8021441ad) |
| Aric Stewart | 2006-01-13 | [wininet: Handle NULL lpBuffersIn in HttpSendRequestExW.](http://source.winehq.org/git/wine.git?a=commitdiff;h=21712d3d156740b18f2d9489ec819fbda41b3b13) |
| Aric Stewart | 2006-01-11 | [winefile: Highlight the file specified on the command line instead of](http://source.winehq.org/git/wine.git?a=commitdiff;h=59b2838f4ea5c0a542a22bb5f622a1999db51429) |
| Aric Stewart | 2006-01-11 | [msvcrt: Modify dir test to create its own directory to ensure the](http://source.winehq.org/git/wine.git?a=commitdiff;h=4bc3b16b449d0508f16f324e82228d752d4792da) |
| Dan Kegel | 2006-01-05 | [oleaut32: Allow \_invoke to handle up to 23 parameters.](http://source.winehq.org/git/wine.git?a=commitdiff;h=d69366a17191fb96b92aecf085561ad047adfd86) |
