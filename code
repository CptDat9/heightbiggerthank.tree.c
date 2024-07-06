int ChieuCaoCay(Tree c)
{
    if (c!=NULL)
    {
        int a = ChieuCaoCay(c->pLeft);
        int b = ChieuCaoCay(c->pRight);
        int max = (a>b)?a:b;
        return 1 + max;
    }
    return 0;
}
int DemTangThuk(Tree c, int k)
{
    if (c!=NULL)
    {
        k--;
        int a = DemTangThuk(c->pLeft,k);
        int b = DemTangThuk(c->pRight,k);
        if (k==0)
            return 1 + a + b;
        return a + b;
    }
    return 0;
}
int Dem(Tree c, int k)
{
    if (c!=NULL)
    {
        int DemSoLuong = 0;
        for (int i=k;i<ChieuCaoCay(c); i++)
        {
            DemSoLuong += DemTangThuk(c,i);
        }
        return DemSoLuong;
    }
    return 0;
}
