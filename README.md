# XMLReader

This project comes from a component developed by Troy Brant , i have add recursion method to remove extra node from the result.


## Usage

	NSData *data = ...; // some data that can be received from remote service
	NSError *error = nil;
	NSDictionary *dict = [XMLReader dictionaryForXMLData:data 
	                                             options:XMLReaderOptionsProcessNamespaces 
	                                               error:&error];
                      
    //method to remove extra node
    NSMutableDictionary *dic_removeKeyNode = [[XMLReader recursionRemoveTextNode:dict] mutableCopy];



## Requirements

Xcode 4.4 and above because project use the "auto-synthesized property" feature.


## FAQ


## Contributions

Thanks to the original author of this component Troy Brant and to [Divan "snip3r8" Visagie](https://github.com/snip3r8) for providing ARC support.


## License

Copyright (C) 2012 Antoine Marcadet

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/amarcadet/XMLReader/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

