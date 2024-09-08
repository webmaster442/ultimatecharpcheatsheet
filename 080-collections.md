# Collections

^^^
![collection interfaces](img/collections1.svg)
^^^ collection interfaces

|                 Type                 |                                                              Description                                                               |                                     Is                                     |
| :----------------------------------: | :------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------: |
|                `T[]`                 |                                                          Represents an Array                                                           |                       `IList<T>`, `IReadonlyList<T>`                       |
|              `List<T>`               |                               Represents a strongly typed list of objects that can be accessed by index                                |                       `IList<T>`, `IReadonlyList<T>`                       |
|      `Dictionary<TKey, TValue>`      |                                               Represents a collection of keys and values                                               |      `IReadOnlyDictionary<TKey, TValue>`, `IDictionary<TKey, TValue>`      |
|             `HashSet<T>`             |                                                       Represents a set of values                                                       |                        `ISet<T>`, `IReadOnlySet<T>`                        |
|              `Queue<T>`              |                                              Represents a first-in, first-out collection                                               |                 `ICollection<T>`, `IReadOnlyCollection<T>`                 |
| `PriorityQueue<TElement, TPriority>` |                                     On Dequeue the item with the lowest priority value is removed                                      |                                     --                                     |
|              `Stack<T>`              |                                     Represents a variable size last-in-first-out (LIFO) collection                                     |                 `ICollection<T>`, `IReadOnlyCollection<T>`                 |
|           `LinkedList<T>`            |                                                    Represents a doubly linked list                                                     |                 `ICollection<T>`, `IReadOnlyCollection<T>`                 |
|           `Collection<T>`            |                                           Provides the base class for a generic collection.                                            | `ICollection<T>`, `IReadOnlyCollection<T>`, `IList<T>`, `IReadonlyList<T>` |
|       `ReadOnlyCollection<T>`        |                                      Provides the base class for a generic read-only collection.                                       | `ICollection<T>`, `IReadOnlyCollection<T>`, `IList<T>`, `IReadonlyList<T>` |
|      `ObservableCollection<T>`       | Represents a dynamic data collection that provides notifications when items get added or removed, or when the whole list is refreshed. |   `Collection<T>`, `INotifyCollectionChanged`, `INotifyPropertyChanged`    |
|           `BindingList<T>`           |                                       Provides a generic collection that supports data binding.                                        |                              `ICollection<T>`                              |
|   `FrozenDictionary<TKey,TValue>`    |                         Provides an immutable, read-only dictionary optimized for fast lookup and enumeration.                         |      `IReadOnlyDictionary<TKey, TValue>`, `IDictionary<TKey, TValue>`      |
|            `FrozenSet<T>`            |                            Provides an immutable, read-only set optimized for fast lookup and enumeration.                             |                        `ISet<T>`, `IReadOnlySet<T>`                        |


## Concurrent Collections

|                Type                 |                               Description                               |                                Is                                 |
| :---------------------------------: | :---------------------------------------------------------------------: | :---------------------------------------------------------------: |
|       `BlockingCollection<T>`       | Provides blocking and bounding capabilities for thread-safe collections |                     `IReadOnlyCollection<T>`                      |
|         `ConcurrentBag<T>`          |        Represents a thread-safe, unordered collection of objects        |    `IReadOnlyCollection<T>`, `IProducerConsumerCollection<T>`     |
| `ConcurrentDictionary<TKey,TValue>` |         Represents a thread-safe collection of key/value pairs          | `IReadOnlyDictionary<TKey,TValue>`,  ` IDictionary<TKey,TValue> ` |
|        `ConcurrentQueue<T>`         |      Represents a thread-safe first in-first out (FIFO) collection      |    `IReadOnlyCollection<T>`, `IProducerConsumerCollection<T>`     |
|        `ConcurrentStack<T>`         |      Represents a thread-safe last in-first out (LIFO) collection       |    `IReadOnlyCollection<T>`, `IProducerConsumerCollection<T>`     |
