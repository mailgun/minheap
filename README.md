minheap
=======

Slightly more user-friendly heap on top of containers/heap.

```go

func toEl(i int) interface{} {
	return &i
}

func fromEl(i interface{}) int {
	return *(i.(*int))
}

mh := NewMinHeap()

el := &Element{
   Value:    toEl(1),
   Priority: 5,
}

mh.PushEl(el)
mh.PeekEl()
mh.Len()
mh.PopEl()

```
