


## テンプレートを使用して仮想マシンにタグを付ける
まず、テンプレートを使用してタグを付けてみましょう。[このテンプレート](https://github.com/Azure/azure-quickstart-templates/tree/master/101-vm-tags)では、Compute (仮想マシン)、Storage (ストレージ アカウント)、および Network (パブリック IP アドレス、Virtual Network、およびネットワーク インターフェイス) というリソースにタグを設定します。このテンプレートは Windows VM のものですが、Linux VM 用に調整できます。

[テンプレート リンク](https://github.com/Azure/azure-quickstart-templates/tree/master/101-vm-tags)から **[Azure へのデプロイ]** ボタンをクリックします。[Azure ポータル](https://portal.azure.com/)が開きます。ポータルにはこのテンプレートをデプロイできます。

![タグを使用した単純なデプロイ](./media/virtual-machines-common-tag/deploy-to-azure-tags.png)

このテンプレートには、*Department*、*Application*、および *Created By* というタグが含まれています。別のタグ名を使いたい場合は、テンプレートにタグを追加したり、タグを編集したりすることができます。

![テンプレートの Azure タグ](./media/virtual-machines-common-tag/azure-tags-in-a-template.png)

上の例のように、タグはキーと値のペアとして定義され、コロン (:) で区切られています。タグは次の形式で定義する必要があります。

        “tags”: {
            “Key1” : ”Value1”,
            “Key2” : “Value2”
        }

選択したタグの編集を完了したら、テンプレート ファイルを保存します。

次に、**[パラメーターの編集]** セクションで、タグの値を入力します。

![Azure ポータルでタグを編集する](./media/virtual-machines-common-tag/edit-tags-in-azure-portal.png)

**[作成]** をクリックして、タグの値が指定されたこのテンプレートをデプロイします。

## ポータルからタグを付ける
タグを使用してリソースを作成したら、ポータルでタグの表示、追加、および削除を行うことができます。

タグを表示するには、タグ アイコンを選択します。

![Azure ポータルのタグ アイコン](./media/virtual-machines-common-tag/azure-portal-tags-icon.png)

ポータルで新しいタグを追加するには、キーと値のペアを定義して保存します。

![Azure ポータルで新しいタグを追加する](./media/virtual-machines-common-tag/azure-portal-add-new-tag.png)

リソースのタグ一覧に新しいタグが表示されます。

![Azure ポータルで保存された新しいタグ](./media/virtual-machines-common-tag/azure-portal-saved-new-tag.png)

<!---HONumber=AcomDC_0706_2016-->