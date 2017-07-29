# Tableview-Cell-Swipe-Show-Delete-Or-More-Button-In-Swift-3-Xcode-8
This Tutorial. I am Show you Tableview Cell Swipe Show Delete Or More Button In Swift 3 Xcode 8 <br>

Show More Or Delete Button Add One Tableview Method in TableViewController Class <br>

Add this Method in TableViewController.swift Class --> <br>
func tableView(_ tableView: UITableView, editActionsForRowAt indexPath: IndexPath) -> [UITableViewRowAction]? {
}
<br>
<br>
This is Full Code --> <br>
  func tableView(_ tableView: UITableView, editActionsForRowAt indexPath: IndexPath) -> [UITableViewRowAction]? { <br><br>
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; let more = UITableViewRowAction(style: .normal, title: "More",   handler: { action , indexPath in <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; print("More Click SuccessFully") <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; })<br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; let delete = UITableViewRowAction(style: .destructive, title: "Delete", handler: { action , indexPath in <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; print("Delete Click SuccessFully") <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; }) <br><br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; return [more,delete] <br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; } <br>
