# vm_team_furuya
クラスの分け方の説明
（そもそもクラスのメリットは、内部にデータを保持できて、そのデータを利用する独自のメソッドを持てるため下記のように考えた。）

-class Drinkは、商品の情報を初期値としてハッシュで保存しインスタンス化して、種類ごとに取り出せるようにし、クラスメソッドとして使うため。
つまり、ドリンククラス（ドリンクのメニュー）の設計図を設計して、作成して、使用するため。
（たい焼きと中身の概念参考）


-class VendingMachineは、
・実際の自動販売機をメソッド（機能）ごとに分けるために定義している。以下は機能

自動販売機の使い方

・お金の管理
①　「slot_money(money)」で10円玉、50円玉、100円玉、500円玉、1000円札を１つずつ投入できる。
また、現在の投入金額と投入した金額を表示できる。

②　「return_money」で払い戻し操作。返すお金の金額を表示して、自動販売機に入っているお金を0円に戻す。

③　「current_slot_money」で投入金額の総計を取得し、表示する。

④　「current_sales_money」で全部の売り上げ金額所得し、表示する。


・購入機能
①　「buy_drinks_list」でドリンクリストを表示する。

②「select_drink(drink_number)」でドリンクリストからドリンクナンバーを入力すると、購入できる。残金も表示する。
または、残金と在庫がなければ、購入できない。


・在庫機能
① 「update_stock」で現在の在庫数を確認できる。
 

・自動販売機の機能として欲しいもの

在庫の補充機能


