- 👋 Hi, I’m @ezgigny
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
ezgigny/ezgigny is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
//
//  ViewController.swift
//  swiftİfElse
//
//  Created by ezgi güney on 19.02.2022.
//

import UIKit

class ViewController: UIViewController {

    
    @IBOutlet weak var txtNote1: UITextField!
    @IBOutlet weak var txtNote2: UITextField!
    
    @IBOutlet weak var lblResult: UILabel!
    
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view.
        //örnek 1
        //2 adet notbilgisi alalım.
        //eğer ortalaması 50 ve üzeri ise "geçti" değilse "kaldı" yazsın.
        
    }

    @IBAction func btnCalculator(_ sender: Any) {
        //butona tıklandıktan sonra çalışacak olan kısım.
        
        let note1 = txtNote1.text ?? "not giriniz"
        let note2 = txtNote2.text ?? "not giriniz"
        
        let ort = (Int(note1)! + Int(note2)!) / 2
        
        if ort >= 50 {
            lblResult.text = "GEÇTİ"
        } else {
            lblResult.text = "KALDI"
        }

}

}
