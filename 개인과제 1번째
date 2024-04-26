시스템 사용;

네임스페이스 스파르타_던전_텍스트_게임_
{
    내부 클래스 프로그램
    {

        정적 공극 메인 로비()
        {
            콘솔.클리어();
            MyChar 캐릭터  = new MyChar(01, "Warrior", 10, 5, 100, 1500);
            My Inventory inven = 새로운 My Inventory();
            My Shop Shop = 새로운 My Shop();
            콘솔.선 쓰기(""");
            콘솔.WriteLine("스파르타 마을 에 오신 여러분 환영합니다. ");
            콘솔.WriteLine("이곳에서 던전으로 들어가기전 활동을 할 수 있습니다. ");
            콘솔.선 쓰기(""");
            콘솔.WriteLine("1") 상태 보기");
            콘솔.WriteLine("2"). 인벤토리");
            콘솔.WriteLine("3. 상점");
            콘솔.선 쓰기(""");
            콘솔.WriteLine("원하시는 행동을 입력해주세요. ");
            string input = Console.선 읽기();
            if (입력 == "1")
            {
                성격.MyChar() 표시;
                if (character.menu == 0)
                {
                    메인 로비();
                }
            }
            그렇지 않으면 (입력 == "2")
            {
                인빈의Inven() 표시;
                if (inven.menu == 0)
                {
                    메인 로비();
                }
                그렇지 않으면 (입력 == "3")
                {
                    인빈의장비();
                    if (inven.menu == 0)
                    {
                        메인 로비();
                    }
                    그렇지 않으면 (입력 == "4")
                    {
                        샵.Showshop();
                        if (shop.menu == 0)
                        {
                            메인 로비();
                        }
                    }
                }
                또 다른
                {
                    콘솔.WriteLine("잘못된 선택입니다.");
                    실.수면(1000);
                    메인 로비();
                }
            }
        }

        공용 정적 공극 메인(string[] args)
        {
            메인 로비();
        }
    }

    공개수업 마이인벤토리
    {
        공개 목록<string> Inven;
        공개 메뉴
        공개적으로 선택합니다.

        퍼블릭 보이드 클래식 인벤()
        {
            Inven = 새 목록 <string>(;
            string[] 무기 =
            {
                "1", "무쇠갑옷", "Defend : +5", "무쇠로 만들어져 튼튼한 갑옷입니다. ", "2", "스파르타의 창", "Attack : +7", "스파르타의 전사들이 사용했다는 전설의 창입니다.", "3", "낡은 검", "Attack : +2", "쉽게 볼 수 있는 낡은 검 입니다." };
            (inti = 0; i < weapon.길이; i++)
            {
                인벤.Add(weapon[i]);
            }
        }

        퍼블릭 보이드 쇼인벤()
        {
            콘솔.클리어();
            Classic Inven();
            콘솔.WriteLine("인벤토리");
            콘솔.WriteLine("보유 중인 아이템을 관리할 수 있습니다");
            콘솔.선 쓰기(""");
            콘솔.WriteLine("{아이템 목록}");
            콘솔.WriteLine("1") 장착 관리");
            콘솔.WriteLine("0. 나가기");
            콘솔.줄 쓰기("");
            콘솔.WriteLine("원하시는 행동을 입력하시오");
            콘솔.WriteLine(">"),
            메뉴 = int구문 분석(Console).선 읽기();


            콘솔.클리어();
            Classic Inven();
            콘솔.WriteLine("인벤토리 - 장착관리");
            콘솔.WriteLine("보유 중인 아이템을 관리할 수 있습니다.");
            콘솔.WriteLine("{아이템 목록}");
            (inti = 0; i < Inven)의 경우.카운트; i += 3)
            {
                콘솔.WriteLine("\t" + Inven[i] +"\t"+ Inven[i+1] +"\t"+ Inven[i+2] + "\t");
            }

            콘솔.선 쓰기(""");
            콘솔.WriteLine("0. 나가기");
            콘솔.줄 쓰기("");
            콘솔.WriteLine("원하시는 행동을 입력하시오");
            콘솔.WriteLine(">"),
            메뉴 = int구문 분석(Console).선 읽기();
        }

        공용 장치()
        {
            콘솔.클리어();
            Classic Inven();
            콘솔.WriteLine("인벤토리 - 장착관리");
            콘솔.WriteLine("보유 중인 아이템을 관리할 수 있습니다.");
            콘솔.WriteLine("{아이템 목록}");
            콘솔.WriteLine("{아이템 이름}  | {장비 효과} | {장비 설명} ");
            (inti = 0; i < Inven)의 경우.카운트; i += 3)
                (== (i / 3 + 1)을 선택)
                {
                    콘솔.줄 쓰기("[E]" + "[" + (i / 3 + 1) + "]" + "\t" + "Inven[i]" + "\t" + "Inven[i + 1] + "\t" + "\t" + "Inven[i + 2] + "\t");
                }
                또 다른
                {
                    콘솔.WriteLine("["]") + (i / 3 + 1) + """ + ""\t" + "\t" + "Inven[i + 1] + "\t" + "Inven[i + 2] + "\t");
                }

            콘솔.선 쓰기(""");
            콘솔.WriteLine("0. 나가기");
시스템 사용;
            콘솔.WriteLine("원하시는 행동을 입력하시오");
네임스페이스 스파르타_던전_텍스트_게임_
            메뉴 = int구문 분석(Console).선 읽기();
    내부 클래스 프로그램
    }

    공개수업 마이샵()
    {
        공개 목록<string> 상점;
        공개 메뉴
        공개적으로 선택합니다.

        공용 보이드 아머 무기점()
        {
            Shop = 새 목록<string>(;
            끈[] 갑옷 =
            {
                "-1 수련자 갑옷", "Defend : +5", "수련에 도움을 주는 갑옷입니다.", "-2 무쇠갑옷", "Defend : +9", ".무쇠로 만들어져 튼튼한 갑옷입니다.",
                "-3 스파르타의 갑옷", "Defend : +15", "스파르타의 전사들이 사용했다는 전설의 갑옷입니다."
            };
            (inti = 0; i < 방어구)를 위해.길이; i++)
            {
                샵.추가(armor[i]);
            }

            string[] 무기 =
            {
                "낡은 검", "Attack : +2", "쉽게 볼 수 있는 낡은 검 입니다.", "청동 도끼", "Attack : +5", "어디선가 사용됐던거 같은 도끼 입니다.",
                "스파르타의 창", "Attack : +7", "스파르타의 전사들이 사용했다는 전설의 창 입니다."
            };
            (int j = 0; j < weapon.길이; j++)
            {
                샵.Add(weapon[j]);
            }
        }

        공공 공실 쇼샵()
        {
            콘솔.클리어();
            아머 무기 상점();
            콘솔.WriteLine("상점");
            콘솔.WriteLine("필요한 아이템을 얻을 수 있는 상점 입니다. ");
            콘솔.WriteLine("{아이템 목록}");
            콘솔.WriteLine("{아이템 이름}      | {장비 효과} | {장비 설명} ");
            (inti = 0; i < Shop.카운트; i += 3)
            {
                콘솔.줄 쓰기("\t" + Shop[i] + "\t" + "\t" + Shop[i + 1] + "\t" + Shop[i + 2] + "\t");
            }

            (int j = 0; j < Shop.카운트; j + = 3)
            {
                콘솔.줄 쓰기("\t" + 상점[j] + "\t" + 상점[j + 1] + "\t" + 상점[+2] + "\t");
            }

            콘솔.선 쓰기(""");
            콘솔.WriteLine("0. 나가기");
            콘솔.줄 쓰기("");
            콘솔.WriteLine("원하시는 행동을 입력하시오");
            콘솔.WriteLine(">"),
            메뉴 = int구문 분석(Console).선 읽기();
        }
    }
}
공개수업 마이차르
{
    공개 Lv {get; }
    공용 문자열 Chad {get; }
    공개 공격 {get; }
    공개 변호 {get; }
    공개 HP {get; }
    public int Gold {get; }
    공개 메뉴

    public MyChar(int_Lv, string_Chad, int_Attack, int_Defense, int_HP, int_Gold)
    {
        Lv = _Lv;
        Chad = _Chad;
        공격 = _공격;
        Defense = _Defense;
        HP = _HP;
        Gold = _Gold;
    }

    공용 공백 Show MyChar()
    {
        콘솔.클리어();
        콘솔.WriteLine("상태 보기");
        콘솔.쓰기 라인($"Lv: {Lv}");
        콘솔.쓰기 라인($"Chad: {"전사"});
        콘솔.WriteLine($"공격력: {Attack}");
        콘솔.쓰기 라인($"방어력: {Defend}");
        콘솔.쓰기 라인($"체력: {HP}");
        콘솔.쓰기 선($"Gold: {Gold}");
        콘솔.선 쓰기(""");
        콘솔.WriteLine("0. 나가기");
        콘솔.줄 쓰기("");
        콘솔.WriteLine("원하시는 행동을 입력해주세요");
        콘솔.WriteLine(">"),
        메뉴 = int구문 분석(Console).선 읽기();
    }
}
