# 0day - Type 1 - Class 2 Attack.

Buffer Overflow: - Representation of an Overrun Attack;

Note:
It was p0sixninja who discovered this Access that is running on all iOS 7.x below iBoot Loaders.

+===============================================================================================+
|[8 Bytes of String or Char Code | Plus 2 new Strings of Code] <--------------------------------|
|																				                                                				|
|																				                                                				|
|																				                                                				|
|																				                                                				|
|																				                                                				|
|		[0][0[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]     		|
|																				                                                				|
|			[1][1][1][1][1][1][1][1] = 8 Bytes;												                                |
|			[1][1][1][1][1][1][1][1][1][1] = 10 Bytes;       <--------------Payload-------------------|
|																				                                                				|
|			If the first 2 Bytes, Consists of anew Payload Arbitrary Code;					                  |
|						The Contents can then be altered, and inserted anew.				                      	|
|																				                                                				|
|																				                                                				|
|		[0][0[0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0][0]		      |
|																				                                                				|
|																				                                                				|
|																				                                                				|
|																			                                      +-------------------|
|																			                                      |( C ) _Binary Korra|
+===============================================================================================+
