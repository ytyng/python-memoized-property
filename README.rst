This repository is deprecated.
==============================

You use functools.cached_property.


python-memoized-property
========================

memoized property decorator in python


property デコレータの代わりに使う。
関数の実行を1度だけ行い、計算結果をインスタンス変数として格納しておく。
再度呼び出しが行われた場合、関数をコールせず、インスタンス変数から結果を返す。

slots が定義されているとうまくいかないかもしれない。


.. code-block:: python

  class Hoge(object):
    
      @memoized_property
      def calc(self):
          some cord....
