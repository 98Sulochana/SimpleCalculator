unit Unit1;

interface

uses
  Winapi.Windows, Winapi.Messages, System.SysUtils, System.Variants, System.Classes, Vcl.Graphics,
  Vcl.Controls, Vcl.Forms, Vcl.Dialogs, Vcl.StdCtrls;

type
  TForm1 = class(TForm)
    txtDisplay: TEdit;
    btnBS: TButton;
    btnCE: TButton;
    btnC: TButton;
    btnPM: TButton;
    btnDigit7: TButton;
    btnDigit9: TButton;
    btnAdd: TButton;
    btnDigit4: TButton;
    btnDigit5: TButton;
    btnDigit6: TButton;
    btnSub: TButton;
    btnDigit1: TButton;
    btnDigit2: TButton;
    btnDigit3: TButton;
    btnMult: TButton;
    btnDigit0: TButton;
    btnDot: TButton;
    btnEquals: TButton;
    btnDiv: TButton;
    btnDigit8: TButton;
    procedure NumbersClick(Sender: TObject);
    procedure btnCClick(Sender: TObject);
    procedure btnBSClick(Sender: TObject);
    procedure btnCEClick(Sender: TObject);
    procedure btnPMClick(Sender: TObject);
    procedure btnAddClick(Sender: TObject);
    procedure btnEqualsClick(Sender: TObject);
    procedure btnSubClick(Sender: TObject);
    procedure btnMultClick(Sender: TObject);
  private
    { Private declarations }
    //declare the variable
     firstnum, secondnum, answer: string;
     opers : char;

  public
    { Public declarations }
  end;

var
  Form1: TForm1;

implementation

{$R *.dfm}

procedure TForm1.btnAddClick(Sender: TObject);
begin
   firstnum := txtDisplay.Text;
   opers := '+';
   txtDisplay.Text := '';
end;

procedure TForm1.btnBSClick(Sender: TObject);
begin
txtDisplay.Text := copy(txtDisplay.Text, 1, length(txtDisplay.Text) - 1);

if txtDisplay.Text = '' then
  txtDisplay.Text := '0';
end;

procedure TForm1.btnCClick(Sender: TObject);
begin
txtDisplay.Text := '0';
end;

procedure TForm1.btnCEClick(Sender: TObject);
var f, s: string;
begin

txtDisplay.Text := '0';

f := firstnum;
s := secondnum;

f :='';
s :='';

end;

procedure TForm1.btnEqualsClick(Sender: TObject);
begin
  secondnum := txtDisplay.Text;

  if opers = '+' then
  answer := FloatToStr(StrToFloat(firstnum) + StrToFloat(secondnum));
  txtDisplay.Text := answer;

  if opers = '-' then
  answer := FloatToStr(StrToFloat(firstnum) - StrToFloat(secondnum));
  txtDisplay.Text := answer;

  if opers = '*' then
  answer := FloatToStr(StrToFloat(firstnum) * StrToFloat(secondnum));
  txtDisplay.Text := answer;

end;

procedure TForm1.btnMultClick(Sender: TObject);
begin
firstnum := txtDisplay.Text;
   opers := '*';
   txtDisplay.Text := '';
end;

procedure TForm1.btnPMClick(Sender: TObject);

var q: real;
begin

q := StrToFloat(txtDisplay.Text);

txtDisplay.Text := FloatToStr (-1 * q);

end;

procedure TForm1.btnSubClick(Sender: TObject);
begin
firstnum := txtDisplay.Text;
   opers := '-';
   txtDisplay.Text := '';
end;

procedure TForm1.NumbersClick(Sender: TObject);

//Declare varible
var b: TButton; //Create a object, object name is 'b'

begin

b := Sender as TButton; // Classify the object as a sender

if txtDisplay.Text = '0' then
begin
   txtDisplay.Text := b.Caption;
end
else
   txtDisplay.Text := txtDisplay.Text + b.Caption;
end;

end.

