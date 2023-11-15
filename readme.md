  
<span style="font-family:Arial sans-serif;font-size:16px;">WD Qui bloque</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Cet exemple montre comment signaler aux utilisateurs d'une base de données HFSQL en réseau "qui" bloque un enregistrement inaccessible.</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Dans cet exemple, nous abordons les principaux thèmes suivants :</span>

<span style="font-family:Arial sans-serif;font-size:14px;">1/ la gestion des accès concurrentiels</span>

<span style="font-family:Arial sans-serif;font-size:14px;">2/ le rafraîchissement automatique par timer</span>

<span style="font-family:Arial sans-serif;font-size:14px;">3/ la gestion d'un fichier "système" pour mémoriser des informations sur les verrous posés.</span>

  
<span style="font-family:Arial sans-serif;font-size:14px;">Résumé de l'exemple livré avec WINDEV : </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Cet exemple réalisé avec WINDEV est composé de 2 projets :</span>

<span style="font-family:Arial sans-serif;font-size:14px;">- WD Qui bloque : application de test gérant un fichier "client" en réseau</span>

<span style="font-family:Arial sans-serif;font-size:14px;">- WD Superviseur blocages : outil d'aministration pour visualiser les verrous posés et éventuellement forcer un déblocage.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Un utilisateur peut avoir conservé une fiche de saisie ouverte depuis un certain temps ; ce qui risque de gêner les autres utilisateurs.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Le bouton 'Libérez SVP' permet d'envoyer un message à l'utilisateur concerné pour lui demander de libérer l'enregistrement.</span>

<span style="font-family:Arial sans-serif;font-size:14px;">Le bouton 'Débloquer !' permet de forcer le déblocage de l'enregistrement. </span>

<span style="font-family:Arial sans-serif;font-size:14px;">Attention : Cette opération va envoyer un message forçant la fermeture de l'application ayant effectué le blocage. </span>

  
  
<span style="font-family:Arial sans-serif;font-size:14px;">( \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ ° \_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_ )</span>

  
<span style="font-family:Arial sans-serif;font-size:10px;">Conditions d'utilisation :</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Le programme est fourni dans un but didactique.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">L'utilisation de ce programme s'effectue sous la responsabilité de son utilisateur. La responsabilité de PC SOFT ne pourra en aucun cas être mise en cause si le programme ne fonctionne pas tel que vous l'attendez, ou pour quelque raison que ce soit. </span>

<span style="font-family:Arial sans-serif;font-size:10px;">Tout détenteur d'une licence WINDEV 28 enregistrée est autorisé à modifier ce programme, et est autorisé à l'inclure dans une ou plusieurs de ses applications. Dans ces cas, toute mention se rapportant à PC SOFT, à WinDev ou à WebDev devra être supprimée, afin qu'aucun doute ne puisse subsister dans l'esprit d'un utilisateur final.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Il est interdit de diffuser ou vendre ce programme exemple sans modification substantielle, ou sans l'inclure dans une application de taille substantielle.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Le support technique pour ce programme exemple est accessible à travers le service "Assistance Directe" uniquement.</span>

<span style="font-family:Arial sans-serif;font-size:10px;">Attention: si plusieurs personnes sont susceptibles d'avoir consulté ce programme, il se peut que le programme ait été modifié! </span>

<span style="font-family:Arial sans-serif;font-size:10px;">Assurez-vous d'étudier une version originale de ce programme.</span>

  
  