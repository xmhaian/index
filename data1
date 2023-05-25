using System;
using System.Collections;
using System.Configuration;
using System.Data;
using System.Linq;
using System.Web;
using System.Web.Security;
using System.Web.UI;
using System.Web.UI.HtmlControls;
using System.Web.UI.WebControls;
using System.Web.UI.WebControls.WebParts;
using System.Xml.Linq;

public partial class text_001 : System.Web.UI.Page
{
    protected void Page_Load(object sender, EventArgs e)
    {

    }
    protected void Button1_Click(object sender, EventArgs e)
    {

           //DataSourceSelectArguments ee = new DataSourceSelectArguments();
           //DataView tmp = (DataView)this.SqlDataSource1.Select(ee);
           //TextBox1.Text = tmp[2][0].ToString();

        // 从页面控件 SqlDataSource1 中读取数据
           int i = Convert.ToInt32 ( DropDownList1.Text);
           // 先把数据读取到 dataview 视图中, select 必须要写这个参数 DataSourceSelectArguments.Empty
           //DataView DW1 = (DataView)SqlDataSource1.Select(DataSourceSelectArguments.Empty);

           //DataSourceSelectArguments ee = new DataSourceSelectArguments("操作人 desc, 操作ID Asc ");
           //DataView DW1 = (DataView)SqlDataSource1.Select(ee);

           DataView DW1 = (DataView)SqlDataSource1.Select(DataSourceSelectArguments.Empty);

        // 从视图中读取指定的行 和 列的值 ,行 和 列的顺序编号都是从 0 开始的
           TextBox1.Text = DW1[0]["操作人"].ToString();  //第一行的数值
           TextBox2.Text = DW1[0]["操作ID"].ToString();
           TextBox1.Text = DW1[i]["操作人"].ToString();  //第二行的数值
           TextBox2.Text = DW1[i]["操作ID"].ToString();

       }

}
