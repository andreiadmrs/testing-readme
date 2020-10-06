Interface HTMLAreaElement: HTMLElement{

  attribute DOMString alt;
  attribute DOMString coords;
  attribute DOMString shape;
  attribute DOMString target;
  attribute DOMString download;
  attribute DOMString rel;
  [SameObject, PutForwards=value] readonly attribute DOMTokenList relList;
  attribute DOMString hreflang;
  attribute DOMString type;
  attribute DOMString referrerPollcy;

};

HTMLAreaElement implements
HTMLHyperlinkElementUtlls;
