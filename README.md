Дано интерфейс А у которого 2 метода:
    void setNext(A<T> next);
    A<T> getNext();

На основе этого интерфейса, с помощью метода ListUtils.createStringList() построен односвязный список заполненый буквами
        A -> B -> C -> D -> E -> F -> G

Ваша задача реализовать метод public static<T> A<T> reversion(A<T> node), который будет принимать ссылку
 на первый узел односвязного списка и на выходе возвращал ссылку на первый елемент этого же списка, но после трансформации
 ( метод должен развернуть список, т.е, чтобы его крайний элемент стал первым, предпоследний вторым,
  и т.д, и в конце концов, первый элемент стал бы крайним элементом.)

  и в конечном итоге ваш список должен стать G -> F -> E -> D -> C -> B -> A

  Условием выполнения задачи будет прохождения теста в классе /src/test/java/ua/com/artcode/TestReversion.java