## <a name="what-is"></a>Mobile Services とは
Azure Mobile Services は拡張性の高いモバイル アプリケーション開発プラットフォームです。Azure を使用するとモバイル デバイスのアプリケーションに強化された機能を追加できます。

Mobile Services を使用すると次ができるようになります。

* **ネイティブやクロス プラットフォーム アプリケーションの作成**: iOS、Android、Windows、またはクロス プラットフォームの Xamarin や Cordova (Phonegap) のアプリケーションをネイティブ SDK を使用して、バックエンドのモバイル サービスに接続します。  
* **ユーザーにプッシュ通知を送信**: アプリケーションのユーザーにプッシュ通知を送信します。
* **ユーザーの認証**: Facebook、Twitter などの一般的な ID プロバイダーを利用してアプリケーションのユーザーを認証します。
* **クラウドでのデータの格納**: SQL Database (既定)、Mongo DB、DocumentDB、Azure テーブル、Azure BLOB にユーザー データを保存します。 
* **同期でオフライン対応アプリを構築**: アプリケーションをオフラインで使用できるようにし、Mobile Services を使用してバック グラウンドでデータを同期します。
* **アプリケーションの監視と拡張**: アプリケーションの使用状況を監視し、需要の増加に伴いバックエンドを拡張します。 

## <a name="concepts"></a>Mobile Services の概念
Mobile Services の主要な機能と概念は次のとおりです:

* **アプリケーション キー:** 任意のクライアントからモバイル サービスへのアクセスを制限するために使用する一意の値です。この「キー」はセキュリティ トークンではないので、アプリケーション ユーザーの認証には使用しません。    
* **バックエンド:** アプリケーションをサポートするモバイル サービス インスタンスです。モバイル サービスは、ASP.NET Web API プロジェクト (*.NET backend*) や Node.js プロジェクト (*JavaScript backend*) として実装されます。
* **ID プロバイダー:** Mobile Services で信頼される、アプリケーションのユーザーを認証する外部のサービスです。サポートされているプロバイダーには Facebook、Twitter、Google、Microsoft Account、 Azure Active Directory が含まれます。 
* **プッシュ通知:** Azure Notification Hubs を使用している登録されたデバイスまたはユーザーに送信される、サービスが発信するメッセージです。
* **スケール:** アプリケーションが広く普及した場合に、処理能力、パフォーマンス、ストレージを有償で補強追加する機能です。
* **スケジュールされたジョブ:** 事前に設定されたスケジュールに基づいて、またはオンデマンドで実行される、カスタム コードです。

詳細については、「[Mobile Services の概念](../articles/mobile-services/mobile-services-concepts-links.md)」を参照してください。

<!---HONumber=AcomDC_0309_2016-->