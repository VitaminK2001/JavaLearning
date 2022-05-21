

## HashMap、HashSet认识

HashSet实现了set接口，它不允许集合中有重复的值，当我们提到HashSet时，第一件事情就是在将对象存储在HashSet之前，要先确保对象重写equals()和hashCode()方法，这样才能比较对象的值是否相等，以确保set中没有储存相等的对象。如果我们没有重写这两个方法，将会使用这个方法的默认实现。public boolean add(Object o) 方法用来在Set中添加元素，当元素重复时则会立即返回false，如果添加成功会返回true.

HashMap实现了Map接口，Map接口对键值进行映射。Map中不允许重复的键，Map接口有两个基本的实现，HashMap和TreeMap。Tree Map保存了对象的排列次序，而HashMap则不能。Hash Map运行键和值为NULL，HashMap是非synchronized的，但collection框架提供方法保证Hash Map synchronized，这样多个线程同时访问HashMap时，能保证只有一个线程更改Map.

https://blog.csdn.net/gzn00417/article/details/104537951